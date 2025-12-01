<script setup>
const benefits = [
  {
    image: 'premium_photo-1678988086439-33af83922142.jpeg',
    title: 'Tree Plant Garden',
    description:
      'A wonder serenity has taken prossession of my entire soul, like these sweet mornings of spring which i enjoy with my whole heart.',
  },
  {
    image: 'premium_photo-1683134371956-256b6eae334e.jpeg',
    title: 'Ready Tree Package',
    description:
      'A wonder serenity has taken prossession of my entire soul, like these sweet mornings of spring which i enjoy with my whole heart.',
  },
  {
    image: 'premium_photo-1677756430413-24becbc9964e.jpeg',
    title: 'Tree Irrigation Ready',
    description:
      'A wonder serenity has taken prossession of my entire soul, like these sweet mornings of spring which i enjoy with my whole heart.',
  },
]

const images = import.meta.glob('../../assets/images/*.jpeg', { eager: true })

function getImage(name) {
  return images[`../../assets/images/${name}`]?.default
}
</script>

<template>
  <div class="benefits-section section">
    <div v-for="benefit in benefits" class="item">
      <div class="image">
        <img :src="getImage(benefit.image)" alt="" />
      </div>
      <div class="content">
        <h3>{{ benefit.title }}</h3>
        <p>
          {{ benefit.description }}
        </p>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.benefits-section {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 1rem;

  @media (max-width: 768px) {
    grid-template-columns: repeat(1, 1fr);
  }

  .item {
    display: flex;
    flex-direction: column;

    &:nth-child(even) image {
      order: 2;
    }

    .image {
      height: 220px;
      aspect-ratio: 16/9;
      img {
        display: block;
        height: 100%;
        width: 100%;
        object-fit: cover;
      }
    }

    .content {
      aspect-ratio: 16/9;
      padding: 1rem;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      text-align: center;
      h3 {
        font-size: 1.2rem;
        margin-bottom: 1rem;
      }

      p {
        font-size: 0.9rem;
        color: var(--text-soft);
      }
    }
  }
}
</style>
