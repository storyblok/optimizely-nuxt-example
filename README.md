<div align="center">
	<a href="https://www.storyblok.com?utm_source=github.com&utm_medium=readme&utm_campaign=optimizely-nuxt" align="center">
		<img src="https://a.storyblok.com/f/88751/1776x360/15e0cf2224/readme-header-optimizely.png" alt="Storyblok Logo">
	</a>
	<h1 align="center">Storyblok Optimizely Nuxt Tutorial</h1>
	<p align="center">Repository for the tutorial about A/B testing with <a href="https://www.storyblok.com?utm_source=github.com&utm_medium=referral&utm_campaign=optimizely-nuxt">Storyblok</a>, Optimizely and Nuxt.</p>
</div>

<p align="center">
  <a href="https://discord.gg/jKrbAMz">
   <img src="https://img.shields.io/discord/700316478792138842?label=Join%20Our%20Discord%20Community&style=appveyor&logo=discord&color=09b3af">
   </a>
  <a href="https://twitter.com/intent/follow?screen_name=storyblok">
    <img src="https://img.shields.io/badge/Follow-%40storyblok-09b3af?style=appveyor&logo=twitter" alt="Follow @Storyblok" />
  </a><br/>
  <a href="https://app.storyblok.com/#!/signup?utm_source=github.com&utm_medium=readme&utm_campaign=optimizely-nuxt">
    <img src="https://img.shields.io/badge/Try%20Storyblok-Free-09b3af?style=appveyor&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAB4AAAAeCAYAAAA7MK6iAAAABGdBTUEAALGPC/xhBQAAADhlWElmTU0AKgAAAAgAAYdpAAQAAAABAAAAGgAAAAAAAqACAAQAAAABAAAAHqADAAQAAAABAAAAHgAAAADpiRU/AAACRElEQVRIDWNgGGmAEd3D3Js3LPrP8D8WXZwSPiMjw6qvPoHhyGYwIXNAbGpbCjbzP0MYuj0YFqMroBV/wCxmIeSju64eDNzMBJUxvP/9i2Hnq5cM1devMnz984eQsQwETeRhYWHgIcJiXqC6VHlFBjUeXgav40cIWkz1oLYXFmGwFBImaDFBHyObcOzdW4aSq5eRhRiE2dgYlpuYoYSKJi8vw3GgWnyAJIs/AuPu4scPGObd/fqVQZ+PHy7+6udPOBsXgySLDfn5GRYYmaKYJcXBgWLpsx8/GPa8foWiBhuHJIsl2DkYQqWksZkDFgP5PObcKYYff//iVAOTIDlx/QPqRMb/YSYBaWlOToZIaVkGZmAZSQiQ5OPtwHwacuo4iplMQEu6tXUZMhSUGDiYmBjylFQYvv/7x9B04xqKOnQOyT5GN+Df//8M59ASXKyMHLoyDD5JPtbj42OYrm+EYgg70JfuYuIoYmLs7AwMjIzA+uY/zjAnyWJpDk6GOFnCvrn86SOwmsNtKciVFAc1ileBHFDC67lzG10Yg0+SjzF0ownsf/OaofvOLYaDQJoQIGix94ljv1gIZI8Pv38zPvj2lQWYf3HGKbpDCFp85v07NnRN1OBTPY6JdRSGxcCw2k6sZuLVMZ5AV4s1TozPnGGFKbz+/PE7IJsHmC//MDMyhXBw8e6FyRFLv3Z0/IKuFqvFyIqAzd1PwBzJw8jAGPfVx38JshwlbIygxmYY43/GQmpais0ODDHuzevLMARHBcgIAQAbOJHZW0/EyQAAAABJRU5ErkJggg==" alt="Follow @Storyblok" />
  </a>
</p>

## 🚀 Usage

### Prerequisites

This repo is making use of the structure described in our [A/B Test Tutorial](https://www.storyblok.com/tp/a-b-test-storyblok-optimizely). Please make sure to read it carefully.
The project itself is modeled after our [5 Minute Nuxt Tutorial](https://www.storyblok.com/tp/headless-cms-nuxtjs), where we describe getting content from Storyblok, the Storyblok Bridge
and dynamic components in detail. Definitely worth a read!

### How to use

For evaluation, set the tokens for Storyblok and Optimizely in the environment variables (or [`.env`](./.env)) respectively. The variables are `OPTIMIZELY_SDK` and `SB_TOKEN`.

Install the dependencies and start the dev environment

```bash
npm i
npm run dev
```

## 🔗 Related Links

- **[What is A/B testing?](https://www.optimizely.com/optimization-glossary/ab-testing/)**: A fantastic article on what A/B testing is, what the process is like and how to deal with SEO.
- **[Storyblok Technologies Hub](https://www.storyblok.com/technologies?utm_source=github.com&utm_medium=referral&utm_campaign=wordpress-importe)**: we prepared technology hubs so that you can find selected beginner tutorials, videos, boilerplates, and even cheatsheets all in one place.

### Support

- Bugs or Feature Requests? [Submit an issue](../../../issues/new);

- Do you have questions about Storyblok or you need help? [Join our Discord Community](https://discord.gg/jKrbAMz).

### Contributing

Please see our [contributing guidelines](https://github.com/storyblok/.github/blob/master/contributing.md) and our [code of conduct](https://www.storyblok.com/trust-center#code-of-conduct?utm_source=github.com&utm_medium=readme&utm_campaign=optimizely-nuxt).
This project use [semantic-release](https://semantic-release.gitbook.io/semantic-release/) for generate new versions by using commit messages and we use the Angular Convention to naming the commits. Check [this question](https://semantic-release.gitbook.io/semantic-release/support/faq#how-can-i-change-the-type-of-commits-that-trigger-a-release) about it in semantic-release FAQ.

### License

This repository is published under the [MIT](./LICENSE) license.
