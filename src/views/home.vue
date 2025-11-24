<template>
  <div class="home">
    <header class="hero">
      <div class="hero__content">
        <p class="hero__eyebrow">Vite 官方中文文档</p>
        <h1>卓越的 Web 开发构建工具</h1>
        <p class="hero__desc">
          Vite 是一个超快的前端构建工具，赋能下一代 Web
          应用的发展——极速的服务启动、轻量快速的模块热替换以及开箱即用的现代特性。
        </p>
        <div class="hero__actions">
          <button class="btn btn--primary">开始</button>
          <button class="btn btn--ghost">GitHub</button>
        </div>
        <div class="hero__tags">
          <span>.html</span>
          <span>.css</span>
          <span>.js</span>
        </div>
      </div>
      <div class="hero__logo">
        <div class="sun"></div>
        <div class="glow"></div>
        <p>Vite Logo</p>
      </div>
    </header>

    <section class="features">
      <article class="feature-card">
        <h3>重新诠释开发者体验</h3>
        <p>Vite 让 Web 开发重回简单。</p>
      </article>
      <article class="feature-card">
        <h4>极速的服务启动</h4>
        <p>使用原生 ESM 文件，无需打包即可即时启动。</p>
      </article>
      <article class="feature-card">
        <h4>轻量快速的 HMR</h4>
        <p>无论项目规模，模块热替换始终快速稳定。</p>
      </article>
      <article class="feature-card">
        <h4>开箱即用</h4>
        <p>TypeScript、JSX、CSS 等现代特性直接可用。</p>
      </article>
      <article class="feature-card">
        <h4>优化构建</h4>
        <p>Rollup 预配置构建，支持多页或库模式。</p>
      </article>
    </section>

    <section class="code-block">
      <div class="code-block__badge">灵活的插件系统</div>
      <pre><code>import { createServer } from 'vite'

const server = await createServer({
  // user config options
})

await server.listen()
server.printUrls()</code></pre>
      <p>
        完全类型化的 API，扩展 Rollup 插件接口，并提供 SSR、构建工具化等能力。
      </p>
    </section>

    <section class="ecosystem">
      <div>
        <h3>共同构建的坚实基础</h3>
        <p>
          灵活的插件系统与一流的 SSR 支持，让你可以在 Vite 之上构建任何框架。
        </p>
      </div>
      <div class="ecosystem__grid">
        <div class="ecosystem__item">
          <span>SSR</span>
          <p>设置自定义 SSR 或自建框架从未如此简单。</p>
        </div>
        <div class="ecosystem__item">
          <span>CI Tests</span>
          <p>持续与下游项目联动，稳定迭代。</p>
        </div>
        <div class="ecosystem__item">
          <span>插件生态</span>
          <p>沿袭 Rollup 插件接口，额外提供开发时能力。</p>
        </div>
      </div>
    </section>

    <section class="community">
      <h3>深受社区喜爱</h3>
      <p>“不要只听我们说 —— 来听听 Vite 社区成员的声音”</p>
      <div class="community__quotes">
        <article>
          <p>
            “Vite 是一个系统，让我们可以在 SolidStart
            上构建一个插件驱动的生态。社区令人惊叹。”
          </p>
          <span>— Ryan Carniato</span>
        </article>
        <article>
          <p>
            “Vite 基本上是 JavaScript 的联合国，我会作为 Svelte 的代表出席。”
          </p>
          <span>— Rich Harris</span>
        </article>
        <article>
          <p>“每次以为 Vite 做不到的时候，我都被打脸。它改变了行业。”</p>
          <span>— Jason Miller · David Cramer</span>
        </article>
      </div>
    </section>

    <section class="cta">
      <div>
        <h3>使用 Vite 开始构建</h3>
        <p>准备好迎接一个能跟上您思维速度的开发环境。</p>
      </div>
      <button class="btn btn--primary btn--large">开始</button>
    </section>
  </div>
</template>

<style scoped>
:global(body) {
  margin: 0;
  font-family: "Inter", "PingFang SC", system-ui, -apple-system,
    BlinkMacSystemFont, "Segoe UI", sans-serif;
  color: #0f172a;
  background: #f8fafc;
}

.home {
  padding: 4rem clamp(1.5rem, 5vw, 4rem) 6rem;
  display: flex;
  flex-direction: column;
  gap: 4rem;
}

.hero {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 3rem;
  align-items: center;
}

.hero__content h1 {
  font-size: clamp(2.5rem, 6vw, 4.6rem);
  margin: 0.8rem 0 1rem;
}

.hero__desc {
  font-size: 1.1rem;
  color: #334155;
  max-width: 640px;
}

.hero__actions {
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
  margin: 2rem 0;
}

.btn {
  border: none;
  border-radius: 999px;
  padding: 0.9rem 1.8rem;
  font-size: 1rem;
  font-weight: 600;
  cursor: pointer;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.btn--primary {
  background: linear-gradient(120deg, #7b5dff, #ff4dd2);
  color: #fff;
  box-shadow: 0 15px 35px rgba(123, 93, 255, 0.35);
}

.btn--ghost {
  background: transparent;
  border: 1px solid rgba(15, 23, 42, 0.2);
  color: #0f172a;
}

.btn--large {
  padding: 1.1rem 2.8rem;
  font-size: 1.1rem;
}

.btn:hover {
  transform: translateY(-3px);
}

.hero__tags {
  display: flex;
  gap: 0.75rem;
  color: #475569;
  font-weight: 600;
}

.hero__logo {
  position: relative;
  aspect-ratio: 1;
  border-radius: 1.5rem;
  background: radial-gradient(
    circle at 30% 20%,
    rgba(255, 255, 255, 0.9),
    rgba(238, 242, 255, 0.4)
  );
  overflow: hidden;
  display: grid;
  place-items: center;
  text-transform: uppercase;
  letter-spacing: 0.3em;
  color: #6366f1;
}

.hero__logo .sun {
  width: 40%;
  height: 40%;
  border-radius: 35% 65% 55% 45%;
  background: linear-gradient(135deg, #ffd166, #ff8a5c);
  animation: rotate 8s linear infinite;
}

.hero__logo .glow {
  position: absolute;
  inset: 10%;
  border-radius: 50%;
  background: radial-gradient(
    circle,
    rgba(255, 214, 102, 0.35),
    transparent 60%
  );
  animation: pulse 6s ease-in-out infinite;
}

.features {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 1.25rem;
}

.feature-card {
  padding: 1.5rem;
  border-radius: 1.25rem;
  border: 1px solid rgba(15, 23, 42, 0.08);
  background: #fff;
  box-shadow: 0 20px 35px rgba(15, 23, 42, 0.05);
  transition: transform 0.3s ease, border 0.3s ease;
}

.feature-card--primary {
  background: linear-gradient(135deg, #eef2ff, #fce7f3);
}

.feature-card:hover {
  transform: translateY(-6px);
  border-color: rgba(99, 102, 241, 0.6);
}

.code-block {
  border-radius: 1.5rem;
  background: #0f172a;
  color: #e2e8f0;
  padding: 2rem;
  box-shadow: 0 30px 60px rgba(15, 23, 42, 0.35);
}

.code-block__badge {
  display: inline-flex;
  padding: 0.3rem 0.85rem;
  border-radius: 999px;
  border: 1px solid rgba(255, 255, 255, 0.3);
  margin-bottom: 1rem;
  font-size: 0.85rem;
  letter-spacing: 0.08em;
}

.code-block pre {
  margin: 0;
  font-family: "JetBrains Mono", "Fira Code", monospace;
  overflow-x: auto;
  line-height: 1.65;
}

.ecosystem {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
  gap: 2rem;
  align-items: center;
}

.ecosystem__grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(160px, 1fr));
  gap: 1rem;
}

.ecosystem__item {
  border-radius: 1rem;
  border: 1px solid rgba(15, 23, 42, 0.08);
  padding: 1.2rem;
  background: #fff;
  min-height: 130px;
}

.ecosystem__item span {
  font-weight: 600;
  color: #4338ca;
}

.community {
  text-align: center;
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
}

.community__quotes {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 1rem;
}

.community__quotes article {
  background: #fff;
  border-radius: 1.25rem;
  padding: 1.5rem;
  border: 1px solid rgba(15, 23, 42, 0.08);
  box-shadow: 0 30px 60px rgba(15, 23, 42, 0.05);
}

.cta {
  border-radius: 1.5rem;
  background: linear-gradient(
    120deg,
    rgba(124, 58, 237, 0.12),
    rgba(236, 72, 153, 0.15)
  );
  padding: 2.5rem;
  display: flex;
  align-items: center;
  justify-content: space-between;
  flex-wrap: wrap;
  gap: 1rem;
}

@keyframes rotate {
  from {
    transform: rotate(0deg);
  }
  to {
    transform: rotate(360deg);
  }
}

@keyframes pulse {
  0%,
  100% {
    transform: scale(1);
    opacity: 0.6;
  }
  50% {
    transform: scale(1.15);
    opacity: 0.85;
  }
}

@media (max-width: 768px) {
  .home {
    padding: 3rem 1.25rem 4rem;
  }

  .hero__actions {
    flex-direction: column;
  }

  .cta {
    flex-direction: column;
    align-items: flex-start;
  }
}
</style>
