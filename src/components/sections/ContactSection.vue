<script setup></script>

<template>
  <div id="#contact-us" class="contact-us">
    <form class="inputs section">
      <h1>Contact Us</h1>
      <p>Send us an email with your question or problem to help you!</p>
      <input type="email" placeholder="email" />
      <textarea placeholder="message"></textarea>
      <input type="submit" value="SEND" />
    </form>
    <img src="@/assets/images/photo-1697269520489-2de855272308.jpeg" alt="" />
  </div>
</template>

<style lang="scss" scoped>
.contact-us {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  min-height: 300px;
  overflow: hidden;

  .inputs {
    display: flex;
    flex-direction: column;
    text-align: start;
    gap: 0.25rem;

    h1 {
      font-size: 2rem;
    }

    p {
      color: var(--text-soft);
      margin-bottom: 1.5rem;
    }

    input[type='email'],
    textarea {
      background: none;
      border: 1px solid var(--accent);
      padding: 8px 16px;
      border-radius: 0.25rem;
    }

    input[type='submit'] {
      padding: 12px 24px;
      background: var(--accent);
      border: none;
      border-radius: 0.25px;
      color: white;
      cursor: pointer;

      &:hover {
        background-color: var(--accent-soft);
      }
    }

    input[type='email'] {
      max-width: 300px;
    }

    textarea {
      min-height: 100px;
    }
  }

  img {
    width: 100%;
    height: 100%;
    display: block;
    object-fit: cover;
  }
}
</style>
