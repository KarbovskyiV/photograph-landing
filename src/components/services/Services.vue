<template>
  <div class="services-container">
    <BaseHeader name="Services" />

    <section>
      <ul class="dropdown-menu">
        <li>
          <a
            class="dropdown-item"
            href="#"
            :style="isOpen(1) ? 'border-width: 1px 0 0 0' : 'border-width: 1px 0 1px 0'"
            @click.prevent="toggleDropdown(1)"
          >
            <span class="title">Portraits</span>
            <span class="math-sign">{{ isOpen(1) ? '-' : '+' }}</span>
          </a>
          <Transition name="dropdown">
            <div v-if="isOpen(1)" class="dropdown-content" id="dropdown-1">
              <p>STANDARD PERSONAL PORTRAIT: $250</p>
              <ul>
                <li>
                  <Subtract />
                  1-hour session
                </li>
                <li>
                  <Subtract />
                  One location
                </li>
                <li>
                  <Subtract />
                  20 professionally edited images
                </li>
              </ul>
              <p class="mt-3">STANDARD PERSONAL PORTRAIT: $250</p>
              <ul>
                <li>
                  <Subtract />
                  2-hour session
                </li>
                <li>
                  <Subtract />
                  Multiple locations or outfit changes
                </li>
                <li>
                  <Subtract />
                  40 professionally edited images
                </li>
              </ul>
            </div>
          </Transition>
        </li>
        <li>
          <a
            class="dropdown-item"
            href="#"
            :style="isOpen(2) ? 'border-width: 1px 0 0 0' : 'border-width: 1px 0 1px 0'"
            @click.prevent="toggleDropdown(2)"
          >
            <span class="title">Personal</span>
            <span class="math-sign">{{ isOpen(2) ? '-' : '+' }}</span>
          </a>
          <div v-if="isOpen(2)" class="dropdown-content" id="dropdown-2">
            <p>STANDARD PERSONAL PORTRAIT: $250</p>
            <ul>
              <li>
                <Subtract />
                1-hour session
              </li>
              <li>
                <Subtract />
                One location
              </li>
              <li>
                <Subtract />
                20 professionally edited images
              </li>
            </ul>
            <p class="mt-3">STANDARD PERSONAL PORTRAIT: $250</p>
            <ul>
              <li>
                <Subtract />
                2-hour session
              </li>
              <li>
                <Subtract />
                Multiple locations or outfit changes
              </li>
              <li>
                <Subtract />
                40 professionally edited images
              </li>
            </ul>
          </div>
        </li>
        <li>
          <a
            class="dropdown-item"
            href="#"
            :style="isOpen(3) ? 'border-width: 1px 0 0 0' : 'border-width: 1px 0 1px 0'"
            @click.prevent="toggleDropdown(3)"
          >
            <span class="title">Love</span>
            <span class="math-sign">{{ isOpen(3) ? '-' : '+' }}</span>
          </a>
          <div v-if="isOpen(3)" class="dropdown-content" id="dropdown-3">
            <p>STANDARD PERSONAL PORTRAIT: $250</p>
            <ul>
              <li>
                <Subtract />
                1-hour session
              </li>
              <li>
                <Subtract />
                One location
              </li>
              <li>
                <Subtract />
                20 professionally edited images
              </li>
            </ul>
            <p class="mt-3">STANDARD PERSONAL PORTRAIT: $250</p>
            <ul>
              <li>
                <Subtract />
                2-hour session
              </li>
              <li>
                <Subtract />
                Multiple locations or outfit changes
              </li>
              <li>
                <Subtract />
                40 professionally edited images
              </li>
            </ul>
          </div>
        </li>
      </ul>
      <div class="image-container" :style="{ marginTop: `${219 + dropdownHeight}px` }">
        <img class="image-cover" src="../../assets/services/orange-peony.png" alt="Orange peony" />
      </div>

      <ButtonWithHover name="Order a photo shoot" margin-top="212" margin-left="690" />
    </section>
  </div>
</template>

<script setup>
import BaseHeader from '@/components/headers/BaseHeader.vue';
import { nextTick, ref } from 'vue';
import Subtract from '@/components/icons/Subtract.vue';
import ButtonWithHover from '@/components/buttons/ButtonWithHover.vue';

const openDropdown = ref(null);

const isOpen = (id) => {
  return openDropdown.value === id;
};

const dropdownHeight = ref(0);

const getDropdownHeight = (id) => {
  const dropdown = document.querySelector(`#dropdown-${id}`);
  if (dropdown) {
    return dropdown.getBoundingClientRect().height;
  }
  return 0;
};

const updateDropdownHeight = (id) => {
  dropdownHeight.value = getDropdownHeight(id);
};

const toggleDropdown = (id) => {
  if (openDropdown.value === id) {
    openDropdown.value = null;
    dropdownHeight.value = 0;
  } else {
    openDropdown.value = id;
    nextTick(() => {
      updateDropdownHeight(id);
    });
  }
};
</script>

<style scoped>
@import '@/assets/global.css';

.services-container {
  display: flex;
  align-items: center;
  flex-direction: column;
  margin-top: 120px;

  section {
    margin-top: 60px;
    display: flex;
    max-width: 1130px;

    .dropdown-menu {
      display: flex;
      flex-direction: column;
      padding: 0;
      background-color: #0c1813;
      width: 100%;
      max-width: 1130px;

      /* Transition styles */
      .dropdown-enter-from,
      .dropdown-leave-to {
        opacity: 0;
      }

      .dropdown-enter-active,
      .dropdown-leave-active {
        transition: opacity 1s ease-out;
      }

      .dropdown-enter-to,
      .dropdown-leave-from {
        opacity: 1;
      }

      .dropdown-item {
        display: flex;
        justify-content: space-between;
        padding: 10px;
        border: solid #a7a7a7;
        border-width: 1px 0 1px 0;
        font-family: 'Montserrat';

        .title {
          color: #e5e1d2;
        }

        .math-sign {
          font-size: 18px;
          color: #e5e1d2;
        }

        &:hover,
        &:focus,
        &:active {
          background-color: #0c1813;
        }
      }

      .dropdown-content {
        padding: 0 0 32px 8px;
        color: #e5e1d2;
        font-family: 'Montserrat';
        height: auto;

        ul {
          padding-left: 8px;
        }

        li {
          display: flex;
          align-items: center;
        }

        li svg {
          margin-right: 12px;
        }
      }
    }

    .image-container {
      width: 184px;
      height: 169px;
    }
  }
}
</style>
