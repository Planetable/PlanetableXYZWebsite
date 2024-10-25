+++
title = "Templates"
description = "How to manage and build new templates."
weight = 102
template = "page.html"
+++

## Build New Template

You can create a new template using HTML, CSS, and JS. When the Planet app renders a site, the template can utilize the values provided in the context by the app. The template system is powered by [Stencil](https://github.com/stencilproject/Stencil), a simple yet powerful template language for Swift.

Forking from the default [Plain](https://github.com/Planetable/SiteTemplatePlain) template is an excellent starting point for building your own new template, as it includes most of the code examples you will need.

## Template Browser

You can find all the currently installed templates in Tools -> Template Browser. If you plan to build your own template, [VS Code](https://code.visualstudio.com/) is recommended. After installing VS Code, you can right-click on a template and select "Open in VS Code."

<figure>
  <img src="../../assets/screenshots/template-browser-vscode.png" alt="Template Browser: Open in VS Code" class="screenshot" />
  <figcaption>Tools -&gt; Template Browser -&gt; Open in VS Code</figcaption>
</figure>

## Add Template from GitHub

By default, all templates are stored in the following folder:

```cmd
~/Library/Containers/xyz.planetable.Planet/Data/Documents/Planet/Templates
```

For instance, there is a new work-in-progress template on GitHub:

<a href="https://github.com/Planetable/SiteTemplateCroptop
" target="_blank">https://github.com/Planetable/SiteTemplateCroptop</a>

To add this template to the templates folder, use these commands:

```cmd
cd ~/Library/Containers/xyz.planetable.Planet/Data/Documents/Planet/Templates
git clone https://github.com/Planetable/SiteTemplateCroptop croptop
```

Once a new template has been added to the templates folder, you must restart the app for it to be recognized.

After the new template is recognized, you can find it in the Template Browser under the Tools menu, or you can choose to use it from the Edit Planet option.

<figure>
  <img src="../../assets/screenshots/template-browser.png" alt="Template Browser" class="screenshot" />
  <figcaption>Tools -&gt; Template Browser</figcaption>
</figure>

<figure>
  <img src="../../assets/screenshots/select-template.png" alt="Select Template" class="screenshot" />
  <figcaption>Edit Planet -&gt; Select Template</figcaption>
</figure>

## Built-in Templates

These are the built-in templates in the folder:

- [plain](https://github.com/Planetable/SiteTemplatePlain)
- [sepia](https://github.com/Planetable/SiteTemplateSepia)
- [gamedb](https://github.com/Planetable/SiteTemplate8bit)
- [grid](https://github.com/Planetable/SiteTemplateGrid)

When the app updates, it will attempt to update these templates as well. However, if a .git subfolder is detected, it indicates the folder could be part of the developer environment, and the app will not overwrite it.

### Template Showcase: Plain

This is the default template. It resembles a minimalist operating system look and feel. It features both dark and light modes.

- Live Demo: [planetable.eth](https://planetable.eth.limo)
- Source Code: [Planetable/SiteTemplatePlain](https://github.com/Planetable/SiteTemplatePlain)

<figure>
  <img src="../../assets/templates/plain.png" alt="Template: Plain" class="screenshot" />
  <figcaption>planetable.eth with the Plain template</figcaption>
</figure>

### Template Showcase: Sepia

Sepia is designed for microblogging and rich media content.

- Live Demo: [sol.build](https://sol.build/)
- Source Code: [Planetable/SiteTemplateSepia](https://github.com/Planetable/SiteTemplateSepia)

<figure>
  <img src="../../assets/templates/sepia.png" alt="Template: Sepia" class="screenshot" />
  <figcaption>sol.build with the Sepia template</figcaption>
</figure>

### Template Showcase: Grid

If your blog consists of many photos, this is the template for you. It features both dark and light modes.

- Live Demo: [yihanphotos.eth](https://yihanphotos.eth.limo)
- Source Code: [Planetable/SiteTemplateGrid](https://github.com/Planetable/SiteTemplateGrid)

<figure>
  <img src="../../assets/templates/grid.png" alt="Template: Grid" class="screenshot" />
  <figcaption>yihanphotos.eth with the Grid template</figcaption>
</figure>

### Template Showcase: 8-bit

This experimental template demonstrates that complex JS and graphics are possible with Planet templates. It has a retro gaming vibe.

- Live Demo: [gamedb.eth](https://gamedb.eth.limo)
- Source Code: [Planetable/SiteTemplate8bit](https://github.com/Planetable/SiteTemplate8bit)

<figure>
  <img src="../../assets/templates/8-bit.png" alt="Template: 8-bit" class="screenshot" />
  <figcaption>gamedb.eth with the 8-bit template</figcaption>
</figure>