<template>
  <section class="about">
    <header class="about__hero">
      <h1>关于我们</h1>
      <p>在这里介绍团队或项目的背景信息。</p>
    </header>

    <main class="about__content">
      <article class="about__section">
        <h2>我们的使命</h2>
        <p>概述产品或服务想要解决的问题与价值。</p>
      </article>
      <article class="about__section">
        <h2>团队成员</h2>
        <p>可以列举核心成员或合作伙伴的简介。</p>
      </article>
    </main>
  </section>
</template>

<style scoped>
.about {
  display: flex;
  flex-direction: column;
  gap: 2rem;
  padding: 2rem;
}

.about__hero {
  text-align: center;
}

.about__content {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
  gap: 1.5rem;
}

.about__section {
  padding: 1.5rem;
  border-radius: 0.75rem;
  border: 1px solid #e2e8f0;
  background-color: #fff;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.06);
}
</style>

