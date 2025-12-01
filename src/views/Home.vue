<script setup>
import TestimonialsSection from '@/components/sections/TestimonialsSection.vue'
import FeaturesSection from '@/components/sections/FeaturesSection.vue'
import GallerySection from '@/components/sections/GallerySection.vue'
import HeroSection from '@/components/sections/HeroSection.vue'
import Navbar from '@/components/ui/Navbar.vue'
import TopServicesSection from '@/components/sections/TopServicesSection.vue'
import BenefitsSection from '@/components/sections/BenefitsSection.vue'
import PackagesSection from '@/components/sections/PackagesSection.vue'
import Footer from '@/components/sections/Footer.vue'
import ContactSection from '@/components/sections/ContactSection.vue'
</script>

<template>
  <Navbar />

  <main>
    <HeroSection />

    <TopServicesSection />

    <FeaturesSection />

    <TestimonialsSection />

    <GallerySection />

    <BenefitsSection />

    <PackagesSection />

    <ContactSection />

    <Footer />
  </main>
</template>

<style lang="scss" scoped></style>
