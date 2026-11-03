<div align="center">

![webforJ: the AI-ready Java web UI framework](./cover.png)

**webforJ is an AI-ready Java web UI framework.** Build modern web apps entirely in Java, bring your existing desktop apps to the web, and let your AI coding assistant build alongside you. Backed by BASIS International's almost 40 years of expertise, including 20+ years of delivering technology built on Java.

[![Latest Release](https://img.shields.io/maven-metadata/v.svg?label=Latest&&color=022495&metadataUrl=https%3A%2F%2Frepo1.maven.org%2Fmaven2%2Fcom%2Fwebforj%2Fwebforj-parent%2Fmaven-metadata.xml)](https://github.com/webforj/webforj/releases)
[![License: MIT](https://img.shields.io/badge/License-MIT-022495)](https://github.com/webforj/webforj/blob/main/LICENSE)

[Get started](https://docs.webforj.com/docs/introduction/getting-started) · [Documentation](https://docs.webforj.com) · [Blog](https://docs.webforj.com/blog) · [Schedule a discovery call](https://webforj.com/schedule-discovery/)

</div>

## Your AI assistant already speaks webforJ

Your assistant doesn't have to guess at webforJ. The [webforJ AI plugin](https://docs.webforj.com/docs/ai-tooling) teaches it the framework in one install, and works with Claude Code, GitHub Copilot, Cursor, Gemini CLI and Codex.

```bash
claude plugin marketplace add webforj/webforj-ai
claude plugin install webforj@webforj-ai
```

- **[MCP server](https://docs.webforj.com/docs/ai-tooling/mcp):** live access to the webforJ docs, project scaffolding, theme generation and design token validation, so answers come from current documentation instead of training data.
- **[Agent Skills](https://docs.webforj.com/docs/ai-tooling/agent-skills):** step-by-step workflows for building forms, creating components, styling apps, securing routes, async work, localization and version upgrades.
- **[MCP Apps](https://docs.webforj.com/docs/integrations/mcp-apps/overview):** open a webforJ view inside an AI app's conversation, so the person and the AI work with the same live UI. Experimental.
- **AI-friendly docs:** every docs page opens in ChatGPT or Claude in one click, and the full documentation is published as [llms.txt](https://docs.webforj.com/llms.txt).

## Edit your running app, visually

[craftforJ](https://docs.webforj.com/docs/craftforj) is the visual development environment that ships with webforJ. It runs inside your app in development mode and shows the components your Java code created.

- **Click and change:** select any component in the page and edit its properties while the app runs.
- **Back to source:** review your live edits as a diff and write the ones you keep into your Java files.
- **Routes and theme:** navigate every route, adjust its access rules, and tune the design tokens with an instant preview.
- **An agent built in:** the [craftforJ assistant](https://docs.webforj.com/docs/ai-tooling/craftforj-assistant) writes Java inside the running app, compiles each change before you see it, and applies it with your approval.

## Swing to web, one screen at a time

Run your existing Swing, JavaFX or SWT app in the browser through [Webswing](https://docs.webforj.com/docs/integrations/webswing/overview), then move it to webforJ one screen at a time. Your users get the web version right away, and your team rewrites at its own pace, in the language it already knows.

BASIS International has spent almost 40 years assisting organizations to modernize mission-critical systems. webforJ brings that experience to your Java apps.

## One design system, every screen

Every webforJ component comes from one design system, so your app looks and behaves consistently from the first screen to the last. Themes, light and dark modes and design tokens are built in, and the [DWC Design Kit for Figma](https://www.figma.com/community/file/1682060886525639971/) lets designers work with the same components your developers use.

## No JavaScript to write. No REST layer. Just Java.

```java
@Route("/")
public class HelloWorldView extends Composite<FlexLayout> {
  private final FlexLayout self = getBoundComponent();
  private final Paragraph hello = new Paragraph("Hello World!");
  private final Button btn = new Button("Say Hello");

  public HelloWorldView() {
    btn.setTheme(ButtonTheme.SUCCESS)
        .addClickListener(e -> showMessageDialog("Hello World!", "Do it all in Java"));

    self.setDirection(FlexDirection.COLUMN).add(hello, btn);
  }
}
```

Generate a ready-to-run project with [startforJ](https://docs.webforj.com/startforj), or follow the [getting started guide](https://docs.webforj.com/docs/introduction/getting-started).

## Build it with us

Found a bug or have an idea? Open an issue in [webforj](https://github.com/webforj/webforj). Not sure where it belongs? Post it there and we'll route it. To contribute code, read the [contributing guide](https://github.com/webforj/webforj/blob/main/CONTRIBUTING.md).

---

<div align="center">

Do it all in Java. Build in Java, deploy to the web.

[webforj.com](https://webforj.com) · [JavaDocs](https://javadoc.io/doc/com.webforj)

</div>
