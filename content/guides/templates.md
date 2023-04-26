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
- [gamedb](https://github.com/Planetable/SiteTemplate8bit)
- [grid](https://github.com/Planetable/SiteTemplateGrid)

When the app updates, it will attempt to update these templates as well. However, if a .git subfolder is detected, it indicates the folder could be part of the developer environment, and the app will not overwrite it.