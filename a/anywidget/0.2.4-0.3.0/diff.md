# Comparing `tmp/anywidget-0.2.4.tar.gz` & `tmp/anywidget-0.3.0.tar.gz`

## Comparing `anywidget-0.2.4.tar` & `anywidget-0.3.0.tar`

### file list

```diff
@@ -1,100 +1,100 @@
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 anywidget-0.2.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 anywidget-0.2.4/anywidget.json
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 anywidget-0.2.4/package.json
--rw-r--r--   0        0        0   251374 2020-02-02 00:00:00.000000 anywidget-0.2.4/pnpm-lock.yaml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 anywidget-0.2.4/pnpm-workspace.yaml
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 anywidget-0.2.4/.changeset/config.json
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 anywidget-0.2.4/anywidget/__init__.py
--rw-r--r--   0        0        0    24459 2020-02-02 00:00:00.000000 anywidget-0.2.4/anywidget/_descriptor.py
--rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 anywidget-0.2.4/anywidget/_file_contents.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 anywidget-0.2.4/anywidget/_protocols.py
--rw-r--r--   0        0        0     6572 2020-02-02 00:00:00.000000 anywidget-0.2.4/anywidget/_util.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 anywidget-0.2.4/anywidget/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anywidget-0.2.4/anywidget/py.typed
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 anywidget-0.2.4/anywidget/widget.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 anywidget-0.2.4/anywidget/labextension/package.json
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 anywidget-0.2.4/anywidget/labextension/static/138.a09415eb66356ea59cee.js
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 anywidget-0.2.4/anywidget/labextension/static/326.968b0416b22301c543f2.js
--rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 anywidget-0.2.4/anywidget/labextension/static/remoteEntry.268da9f8b94063c87ec8.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 anywidget-0.2.4/anywidget/labextension/static/style.js
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 anywidget-0.2.4/anywidget/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 anywidget-0.2.4/anywidget/nbextension/extension.js
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 anywidget-0.2.4/anywidget/nbextension/index.js
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/README.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/astro.config.mjs
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/package.json
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/tailwind.config.cjs
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/tsconfig.json
--rw-r--r--   0        0        0   625221 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/public/anywidget-overview.png
--rw-r--r--   0        0        0   440603 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/public/banner-dark.png
--rw-r--r--   0        0        0   413948 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/public/banner-light.png
--rw-r--r--   0        0        0   101574 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/public/banner-minimal.png
--rw-r--r--   0        0        0   678629 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/public/client-js-diagram.png
--rw-r--r--   0        0        0   748347 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/public/default-og-image.png
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/public/favicon.svg
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/public/make-scrollable-code-focusable.js
--rw-r--r--   0        0        0   275942 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/public/widget-overview.png
--rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/scripts/ipynb.mjs
--rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/scripts/render.py
--rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/scripts/utils.mjs
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/consts.ts
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/env.d.ts
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/languages.ts
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/util.ts
--rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/components/CodeHero.astro
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/components/ConfettiButton.astro
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/components/Counter.astro
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/components/CounterButton.astro
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/components/HeadCommon.astro
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/components/HeadSEO.astro
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/components/Hero.astro
--rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/components/Footer/AvatarList.astro
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/components/Footer/Footer.astro
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/components/Header/AnyWidgetLogo.astro
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/components/Header/AstroLogo.astro
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/components/Header/Header.astro
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/components/Header/HeaderButton.css
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/components/Header/LanguageSelect.css
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/components/Header/LanguageSelect.tsx
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/components/Header/Search.css
--rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/components/Header/Search.tsx
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/components/Header/SidebarToggle.css
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/components/Header/SidebarToggle.tsx
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/components/Header/SkipToContent.astro
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/components/Header/ThemeToggleButton.css
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/components/Header/ThemeToggleButton.tsx
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/components/LeftSidebar/LeftSidebar.astro
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/components/PageContent/PageContent.astro
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/components/RightSidebar/MoreMenu.astro
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/components/RightSidebar/RightSidebar.astro
--rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/components/RightSidebar/TableOfContents.tsx
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/components/examples/Counter.astro
--rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/layouts/MainLayout.astro
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/layouts/SplashLayout.astro
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/pages/index.astro
--rw-r--r--   0        0        0     7638 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/pages/blog/anywidget-02.md
--rw-r--r--   0        0        0    22533 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/pages/blog/introducing-anywidget.mdx
--rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/pages/en/bundling.md
--rw-r--r--   0        0        0     5645 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/pages/en/getting-started.mdx
--rw-r--r--   0        0        0    10676 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/pages/en/jupyter-widgets-the-good-parts.md
--rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/pages/en/notebooks/counter.ipynb
--rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/styles/index.css
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 anywidget-0.2.4/docs/src/styles/theme.css
--rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 anywidget-0.2.4/examples/Counter.ipynb
--rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 anywidget-0.2.4/examples/minimal_example.ipynb
--rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 anywidget-0.2.4/packages/anywidget/CHANGELOG.md
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 anywidget-0.2.4/packages/anywidget/build.mjs
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 anywidget-0.2.4/packages/anywidget/package.json
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 anywidget-0.2.4/packages/anywidget/src/index.js
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 anywidget-0.2.4/packages/anywidget/src/plugin.js
--rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 anywidget-0.2.4/packages/anywidget/src/widget.js
--rw-r--r--   0        0        0     9118 2020-02-02 00:00:00.000000 anywidget-0.2.4/tests/test_descriptor.py
--rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 anywidget-0.2.4/tests/test_file_contents.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anywidget-0.2.4/tests/test_protocols.py
--rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 anywidget-0.2.4/tests/test_utils.py
--rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 anywidget-0.2.4/tests/test_widget.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 anywidget-0.2.4/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 anywidget-0.2.4/LICENSE
--rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 anywidget-0.2.4/README.md
--rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 anywidget-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     5632 2020-02-02 00:00:00.000000 anywidget-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 anywidget-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 anywidget-0.3.0/anywidget.json
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 anywidget-0.3.0/package.json
+-rw-r--r--   0        0        0   251374 2020-02-02 00:00:00.000000 anywidget-0.3.0/pnpm-lock.yaml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 anywidget-0.3.0/pnpm-workspace.yaml
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 anywidget-0.3.0/.changeset/config.json
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 anywidget-0.3.0/anywidget/__init__.py
+-rw-r--r--   0        0        0    24407 2020-02-02 00:00:00.000000 anywidget-0.3.0/anywidget/_descriptor.py
+-rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 anywidget-0.3.0/anywidget/_file_contents.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 anywidget-0.3.0/anywidget/_protocols.py
+-rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 anywidget-0.3.0/anywidget/_util.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 anywidget-0.3.0/anywidget/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anywidget-0.3.0/anywidget/py.typed
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 anywidget-0.3.0/anywidget/widget.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 anywidget-0.3.0/anywidget/labextension/package.json
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 anywidget-0.3.0/anywidget/labextension/static/138.cc3c5434a894a5dab1d2.js
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 anywidget-0.3.0/anywidget/labextension/static/326.065deffd433fe1343e66.js
+-rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 anywidget-0.3.0/anywidget/labextension/static/remoteEntry.73b94c9a97622529eed7.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 anywidget-0.3.0/anywidget/labextension/static/style.js
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 anywidget-0.3.0/anywidget/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 anywidget-0.3.0/anywidget/nbextension/extension.js
+-rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 anywidget-0.3.0/anywidget/nbextension/index.js
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/README.md
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/astro.config.mjs
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/package.json
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/tailwind.config.cjs
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/tsconfig.json
+-rw-r--r--   0        0        0   625221 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/public/anywidget-overview.png
+-rw-r--r--   0        0        0   440603 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/public/banner-dark.png
+-rw-r--r--   0        0        0   413948 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/public/banner-light.png
+-rw-r--r--   0        0        0   101574 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/public/banner-minimal.png
+-rw-r--r--   0        0        0   678629 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/public/client-js-diagram.png
+-rw-r--r--   0        0        0   748347 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/public/default-og-image.png
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/public/favicon.svg
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/public/make-scrollable-code-focusable.js
+-rw-r--r--   0        0        0   275942 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/public/widget-overview.png
+-rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/scripts/ipynb.mjs
+-rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/scripts/render.py
+-rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/scripts/utils.mjs
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/consts.ts
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/env.d.ts
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/languages.ts
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/util.ts
+-rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/CodeHero.astro
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/ConfettiButton.astro
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/Counter.astro
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/CounterButton.astro
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/HeadCommon.astro
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/HeadSEO.astro
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/Hero.astro
+-rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/Footer/AvatarList.astro
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/Footer/Footer.astro
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/Header/AnyWidgetLogo.astro
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/Header/AstroLogo.astro
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/Header/Header.astro
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/Header/HeaderButton.css
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/Header/LanguageSelect.css
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/Header/LanguageSelect.tsx
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/Header/Search.css
+-rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/Header/Search.tsx
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/Header/SidebarToggle.css
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/Header/SidebarToggle.tsx
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/Header/SkipToContent.astro
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/Header/ThemeToggleButton.css
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/Header/ThemeToggleButton.tsx
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/LeftSidebar/LeftSidebar.astro
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/PageContent/PageContent.astro
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/RightSidebar/MoreMenu.astro
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/RightSidebar/RightSidebar.astro
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/RightSidebar/TableOfContents.tsx
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/examples/Counter.astro
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/layouts/MainLayout.astro
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/layouts/SplashLayout.astro
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/pages/index.astro
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/pages/blog/anywidget-02.md
+-rw-r--r--   0        0        0    22533 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/pages/blog/introducing-anywidget.mdx
+-rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/pages/en/bundling.md
+-rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/pages/en/getting-started.mdx
+-rw-r--r--   0        0        0    10676 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/pages/en/jupyter-widgets-the-good-parts.md
+-rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/pages/en/notebooks/counter.ipynb
+-rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/styles/index.css
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/styles/theme.css
+-rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 anywidget-0.3.0/examples/Counter.ipynb
+-rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 anywidget-0.3.0/examples/minimal_example.ipynb
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 anywidget-0.3.0/packages/anywidget/CHANGELOG.md
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 anywidget-0.3.0/packages/anywidget/build.mjs
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 anywidget-0.3.0/packages/anywidget/package.json
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 anywidget-0.3.0/packages/anywidget/src/index.js
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 anywidget-0.3.0/packages/anywidget/src/plugin.js
+-rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 anywidget-0.3.0/packages/anywidget/src/widget.js
+-rw-r--r--   0        0        0     9118 2020-02-02 00:00:00.000000 anywidget-0.3.0/tests/test_descriptor.py
+-rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 anywidget-0.3.0/tests/test_file_contents.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anywidget-0.3.0/tests/test_protocols.py
+-rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 anywidget-0.3.0/tests/test_utils.py
+-rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 anywidget-0.3.0/tests/test_widget.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 anywidget-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 anywidget-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 anywidget-0.3.0/README.md
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 anywidget-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 anywidget-0.3.0/PKG-INFO
```

### Comparing `anywidget-0.2.4/.pre-commit-config.yaml` & `anywidget-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/package.json` & `anywidget-0.3.0/package.json`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/pnpm-lock.yaml` & `anywidget-0.3.0/pnpm-lock.yaml`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/anywidget/_descriptor.py` & `anywidget-0.3.0/anywidget/_descriptor.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 `MimeBundleDescriptor()` takes the place of a `_repr_mimebundle_` method on a class.
 
 - `MimeBundleDescriptor` is a
   [descriptor](https://docs.python.org/3/howto/descriptor.html). When the
   `_repr_mimebundle_` attribute is accessed on an instance of the decorated class, a
   `ReprMimeBundle` instance is created and returned.
 - A `ReprMimeBundle` is first and foremost a callable object that implements the
-  `_repr_mimebundle_` protocol that jupyter expects.  However, it also manages an
-  ipykernel Comm instance that is used to send the state of the python model to the
+  `_repr_mimebundle_` protocol that jupyter expects.  However, it also manages a
+  Comm instance that is used to send the state of the python model to the
   javascript view.  This is done lazily, so that the Comm is only created when the
   `_repr_mimebundle_` is first accessed.
 - `ReprMimeBundle` has the logic to get/set the state of the python model, and will keep
   the two in sync ("bind"/"unbind_instance" methods can be used to control this).
 """
 
 from __future__ import annotations
@@ -35,18 +35,18 @@
     put_buffers,
     remove_buffers,
     try_file_contents,
 )
 from ._version import __version__
 
 if TYPE_CHECKING:  # pragma: no cover
+    import comm
     import psygnal
     import pydantic
     import traitlets
-    from ipykernel.comm import Comm
     from typing_extensions import TypeAlias, TypeGuard
 
     from ._protocols import CommMessage
 
     # catch all for types that can be serialized ... too hard to actually type
     Serializable: TypeAlias = Any
 
@@ -72,31 +72,31 @@
     "_view_module_version": __version__,
     "_view_count": None,
 }
 
 
 def open_comm(
     target_name: str = _TARGET_NAME, version: str = _PROTOCOL_VERSION
-) -> Comm:
-    from ipykernel.comm import Comm
+) -> comm.DummyComm:
+    import comm
 
-    return Comm(  # type: ignore[no-untyped-call]
+    return comm.create_comm(
         target_name=target_name,
         metadata={"version": version},
         data={"state": _ANYWIDGET_STATE},
     )
 
 
 # cache of comms: mapp of id(obj) -> Comm.
 # we use id(obj) rather than WeakKeyDictionary because we can't assume that the
 # object has a __hash__ method
-_COMMS: dict[int, Comm] = {}
+_COMMS: dict[int, comm.DummyComm] = {}
 
 
-def _comm_for(obj: object) -> Comm:
+def _comm_for(obj: object) -> comm.DummyComm:
     """Get or create a communcation channel for a given object.
 
     Comms are cached by object id, so that if the same object is used in multiple
     places, the same comm will be used. Comms are deleted when the object is garbage
     collected.
     """
     # NOTE: this is not a totally safe way to create an id for an object
@@ -242,15 +242,15 @@
 
 
 class ReprMimeBundle:
     """Callable object that behaves like a `_repr_mimebundle_` method...
 
     which is to say, it returns a mimebundle (mapping of mimetypes to data) when called.
 
-    This object *also* controls an ipykernel.Comm channel between the front-end js view
+    This object *also* controls an Comm channel between the front-end js view
     and some python model object (`obj`),
 
     Parameters
     ----------
     obj : object
         The python model object which is being represented by the view.  Most likely
         this will be a dataclass instance that has been made "evented" by the anywidget
```

### Comparing `anywidget-0.2.4/anywidget/_file_contents.py` & `anywidget-0.3.0/anywidget/_file_contents.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/anywidget/_protocols.py` & `anywidget-0.3.0/anywidget/_protocols.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/anywidget/_util.py` & `anywidget-0.3.0/anywidget/_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -160,26 +160,45 @@
 
     if url is None:
         return {}
 
     return {_WIDGET_MIME_TYPE: {"colab": {"custom_widget_manager": {"url": url}}}}
 
 
+def _should_start_thread(path: pathlib.Path) -> bool:
+    if "site-packages" in path.parts:
+        # file is inside site-packages, likely not a local development install
+        return False
+
+    try:
+        import watchfiles  # noqa: F401
+    except ImportError:
+        import warnings
+
+        warnings.warn(
+            "anywidget: Live-reloading feature is disabled."
+            " To enable, please install the 'watchfiles' package.",
+            stacklevel=2,
+        )
+
+        return False
+
+    return True
+
+
 def try_file_contents(x: Any) -> FileContents | None:
     """Try to coerce x into a FileContents object."""
     if not isinstance(x, (str, pathlib.Path)):
         return None
 
     maybe_path = pathlib.Path(x)
 
     # Could raise OSError if not a path and exceeds max path length
     with contextlib.suppress(OSError):
         maybe_path = pathlib.Path(maybe_path).resolve().absolute()
         if maybe_path.is_file():
-            # Start a watch thread if file is outside of site-packages
-            # (i.e., likely a development install)
             return FileContents(
                 path=maybe_path,
-                start_thread="site-packages" not in maybe_path.parts,
+                start_thread=_should_start_thread(maybe_path),
             )
 
     return None
```

### Comparing `anywidget-0.2.4/anywidget/widget.py` & `anywidget-0.3.0/anywidget/widget.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/anywidget/labextension/package.json` & `anywidget-0.3.0/anywidget/labextension/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95703125%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.73b94c9a97622529eed7.js'}}",*

 * * "'version'": "'0.3.0'"}*

```diff
@@ -22,15 +22,15 @@
     },
     "files": [
         "dist"
     ],
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.268da9f8b94063c87ec8.js"
+            "load": "static/remoteEntry.73b94c9a97622529eed7.js"
         },
         "extension": "src/plugin",
         "outputDir": "../../anywidget/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -42,9 +42,9 @@
     "name": "anywidget",
     "publishConfig": {
         "main": "dist/index.js"
     },
     "scripts": {
         "build": "node build.mjs"
     },
-    "version": "0.2.4"
+    "version": "0.3.0"
 }
```

### Comparing `anywidget-0.2.4/anywidget/labextension/static/138.a09415eb66356ea59cee.js` & `anywidget-0.3.0/anywidget/labextension/static/138.cc3c5434a894a5dab1d2.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -92,11 +92,11 @@
                 return {
                     AnyModel: t,
                     AnyView: i
                 }
             }
         },
         147: e => {
-            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.2.4"}')
+            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.3.0"}')
         }
     }
 ]);
```

### Comparing `anywidget-0.2.4/anywidget/labextension/static/326.968b0416b22301c543f2.js` & `anywidget-0.3.0/anywidget/labextension/static/326.065deffd433fe1343e66.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -110,11 +110,11 @@
                 return {
                     AnyModel: t,
                     AnyView: i
                 }
             }
         },
         147: e => {
-            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.2.4"}')
+            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.3.0"}')
         }
     }
 ]);
```

### Comparing `anywidget-0.2.4/anywidget/labextension/static/remoteEntry.268da9f8b94063c87ec8.js` & `anywidget-0.3.0/anywidget/labextension/static/remoteEntry.73b94c9a97622529eed7.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, d, f, s, p, c, h, v = {
+    var e, r, t, n, o, a, i, u, l, f, s, d, p, c, h, v = {
             408: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(138).then((() => () => t(138))),
                         "./extension": () => t.e(326).then((() => () => t(326)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -22,109 +22,109 @@
                     get: () => o,
                     init: () => a
                 })
             }
         },
         g = {};
 
-    function b(e) {
+    function m(e) {
         var r = g[e];
         if (void 0 !== r) return r.exports;
         var t = g[e] = {
             exports: {}
         };
-        return v[e](t, t.exports, b), t.exports
+        return v[e](t, t.exports, m), t.exports
     }
-    b.m = v, b.c = g, b.n = e => {
+    m.m = v, m.c = g, m.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
-        return b.d(r, {
+        return m.d(r, {
             a: r
         }), r
-    }, b.d = (e, r) => {
-        for (var t in r) b.o(r, t) && !b.o(e, t) && Object.defineProperty(e, t, {
+    }, m.d = (e, r) => {
+        for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, b.f = {}, b.e = e => Promise.all(Object.keys(b.f).reduce(((r, t) => (b.f[t](e, r), r)), [])), b.u = e => e + "." + {
-        138: "a09415eb66356ea59cee",
-        326: "968b0416b22301c543f2"
+    }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
+        138: "cc3c5434a894a5dab1d2",
+        326: "065deffd433fe1343e66"
     } [e] + ".js?v=" + {
-        138: "a09415eb66356ea59cee",
-        326: "968b0416b22301c543f2"
-    } [e], b.g = function() {
+        138: "cc3c5434a894a5dab1d2",
+        326: "065deffd433fe1343e66"
+    } [e], m.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), b.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "anywidget:", b.l = (t, n, o, a) => {
+    }(), m.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "anywidget:", m.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== o)
-                for (var l = document.getElementsByTagName("script"), d = 0; d < l.length; d++) {
-                    var f = l[d];
-                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
-                        i = f;
+                for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
+                    var s = l[f];
+                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
+                        i = s;
                         break
                     }
                 }
-            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, b.nc && i.setAttribute("nonce", b.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
-            var s = (r, n) => {
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, m.nc && i.setAttribute("nonce", m.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
+            var d = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(p);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(s.bind(null, void 0, {
+                p = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
-    }, b.r = e => {
+    }, m.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
-        b.S = {};
+        m.S = {};
         var e = {},
             r = {};
-        b.I = (t, n) => {
+        m.I = (t, n) => {
             n || (n = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
                 if (n.push(o), e[t]) return e[t];
-                b.o(b.S, t) || (b.S[t] = {});
-                var a = b.S[t],
+                m.o(m.S, t) || (m.S[t] = {});
+                var a = m.S[t],
                     i = "anywidget",
                     u = [];
                 return "default" === t && ((e, r, t, n) => {
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
-                        get: () => b.e(138).then((() => () => b(138))),
+                        get: () => m.e(138).then((() => () => m(138))),
                         from: i,
                         eager: !1
                     })
-                })("anywidget", "0.2.4"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("anywidget", "0.3.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        b.g.importScripts && (e = b.g.location + "");
-        var r = b.g.document;
+        m.g.importScripts && (e = m.g.location + "");
+        var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
             t.length && (e = t[t.length - 1].src)
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), b.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), m.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
@@ -161,114 +161,114 @@
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var d, f, s = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (f = (typeof(d = r[i]))[0])) return !l || ("u" == s ? u > n && !o : "" == s != o);
-                if ("u" == f) {
-                    if (!l || "u" != s) return !1
+                var f, s, d = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !l || ("u" == d ? u > n && !o : "" == d != o);
+                if ("u" == s) {
+                    if (!l || "u" != d) return !1
                 } else if (l)
-                    if (s == f)
+                    if (d == s)
                         if (u <= n) {
-                            if (d != e[u]) return !1
+                            if (f != e[u]) return !1
                         } else {
-                            if (o ? d > e[u] : d < e[u]) return !1;
-                            d != e[u] && (l = !1)
+                            if (o ? f > e[u] : f < e[u]) return !1;
+                            f != e[u] && (l = !1)
                         }
-                else if ("s" != s && "n" != s) {
+                else if ("s" != d && "n" != d) {
                     if (o || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || f < s != o) return !1;
+                    if (u <= n || s < d != o) return !1;
                     l = !1
-                } else "s" != s && "n" != s && (l = !1, u--)
+                } else "s" != d && "n" != d && (l = !1, u--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
         }
         return !!c()
     }, i = (e, r) => {
-        var t = b.S[e];
-        if (!t || !b.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        var t = m.S[e];
+        if (!t || !m.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", d = (e, r, t, n) => {
+    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
         var o = u(e, t);
-        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(l(e, t, o, n)), f(e[t][o])
-    }, f = e => (e.loaded = 1, e.get()), s = (e => function(r, t, n, o) {
-        var a = b.I(r);
-        return a && a.then ? a.then(e.bind(e, r, b.S[r], t, n, o)) : e(r, b.S[r], t, n)
-    })(((e, r, t, n) => (i(e, t), d(r, 0, t, n)))), p = {}, c = {
-        395: () => s("default", "@jupyter-widgets/base", [, [1, 6],
+        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(l(e, t, o, n)), s(e[t][o])
+    }, s = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, o) {
+        var a = m.I(r);
+        return a && a.then ? a.then(e.bind(e, r, m.S[r], t, n, o)) : e(r, m.S[r], t, n)
+    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), p = {}, c = {
+        395: () => d("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 5],
             [1, 4],
             [1, 3],
             [1, 2], 1, 1, 1, 1
         ])
     }, h = {
         326: [395]
-    }, b.f.consumes = (e, r) => {
-        b.o(h, e) && h[e].forEach((e => {
-            if (b.o(p, e)) return r.push(p[e]);
+    }, m.f.consumes = (e, r) => {
+        m.o(h, e) && h[e].forEach((e => {
+            if (m.o(p, e)) return r.push(p[e]);
             var t = r => {
-                    p[e] = 0, b.m[e] = t => {
-                        delete b.c[e], t.exports = r()
+                    p[e] = 0, m.m[e] = t => {
+                        delete m.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete p[e], b.m[e] = t => {
-                        throw delete b.c[e], r
+                    delete p[e], m.m[e] = t => {
+                        throw delete m.c[e], r
                     }
                 };
             try {
                 var o = c[e]();
                 o.then ? r.push(p[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             957: 0
         };
-        b.f.j = (r, t) => {
-            var n = b.o(e, r) ? e[r] : void 0;
+        m.f.j = (r, t) => {
+            var n = m.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else {
                     var o = new Promise(((t, o) => n = e[r] = [t, o]));
                     t.push(n[2] = o);
-                    var a = b.p + b.u(r),
+                    var a = m.p + m.u(r),
                         i = new Error;
-                    b.l(a, (t => {
-                        if (b.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                    m.l(a, (t => {
+                        if (m.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
                             var o = t && ("load" === t.type ? "missing" : t.type),
                                 a = t && t.target && t.target.src;
                             i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
                 var n, o, [a, i, u] = t,
                     l = 0;
                 if (a.some((r => 0 !== e[r]))) {
-                    for (n in i) b.o(i, n) && (b.m[n] = i[n]);
-                    u && u(b)
+                    for (n in i) m.o(i, n) && (m.m[n] = i[n]);
+                    u && u(m)
                 }
-                for (r && r(t); l < a.length; l++) o = a[l], b.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); l < a.length; l++) o = a[l], m.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkanywidget = self.webpackChunkanywidget || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
-    var m = b(408);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).anywidget = m
+    var b = m(408);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).anywidget = b
 })();
```

### Comparing `anywidget-0.2.4/anywidget/nbextension/index.js` & `anywidget-0.3.0/anywidget/nbextension/index.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 // package.json
 var name = "anywidget";
-var version = "0.2.4";
+var version = "0.3.0";
 
 // src/widget.js
 function is_href(str) {
     return str.startsWith("http://") || str.startsWith("https://");
 }
 async function load_css_href(href, anywidget_id) {
     let prev = document.querySelector(`link[id='${anywidget_id}']`);
```

### Comparing `anywidget-0.2.4/docs/README.md` & `anywidget-0.3.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/astro.config.mjs` & `anywidget-0.3.0/docs/astro.config.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/package.json` & `anywidget-0.3.0/docs/package.json`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/public/anywidget-overview.png` & `anywidget-0.3.0/docs/public/anywidget-overview.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/public/banner-dark.png` & `anywidget-0.3.0/docs/public/banner-dark.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/public/banner-light.png` & `anywidget-0.3.0/docs/public/banner-light.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/public/banner-minimal.png` & `anywidget-0.3.0/docs/public/banner-minimal.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/public/client-js-diagram.png` & `anywidget-0.3.0/docs/public/client-js-diagram.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/public/default-og-image.png` & `anywidget-0.3.0/docs/public/default-og-image.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/public/favicon.svg` & `anywidget-0.3.0/docs/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/public/widget-overview.png` & `anywidget-0.3.0/docs/public/widget-overview.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/scripts/ipynb.mjs` & `anywidget-0.3.0/docs/scripts/ipynb.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/scripts/utils.mjs` & `anywidget-0.3.0/docs/scripts/utils.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/src/consts.ts` & `anywidget-0.3.0/docs/src/consts.ts`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/src/components/CodeHero.astro` & `anywidget-0.3.0/docs/src/components/CodeHero.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/src/components/CounterButton.astro` & `anywidget-0.3.0/docs/src/components/CounterButton.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/src/components/HeadCommon.astro` & `anywidget-0.3.0/docs/src/components/HeadCommon.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/src/components/HeadSEO.astro` & `anywidget-0.3.0/docs/src/components/HeadSEO.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/src/components/Hero.astro` & `anywidget-0.3.0/docs/src/components/Hero.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/src/components/Footer/AvatarList.astro` & `anywidget-0.3.0/docs/src/components/Footer/AvatarList.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/src/components/Header/AnyWidgetLogo.astro` & `anywidget-0.3.0/docs/src/components/Header/AnyWidgetLogo.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/src/components/Header/AstroLogo.astro` & `anywidget-0.3.0/docs/src/components/Header/AstroLogo.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/src/components/Header/Header.astro` & `anywidget-0.3.0/docs/src/components/Header/Header.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/src/components/Header/HeaderButton.css` & `anywidget-0.3.0/docs/src/components/Header/HeaderButton.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/src/components/Header/LanguageSelect.css` & `anywidget-0.3.0/docs/src/components/Header/LanguageSelect.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/src/components/Header/LanguageSelect.tsx` & `anywidget-0.3.0/docs/src/components/Header/LanguageSelect.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/src/components/Header/Search.css` & `anywidget-0.3.0/docs/src/components/Header/Search.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/src/components/Header/Search.tsx` & `anywidget-0.3.0/docs/src/components/Header/Search.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/src/components/Header/SidebarToggle.tsx` & `anywidget-0.3.0/docs/src/components/Header/SidebarToggle.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/src/components/Header/ThemeToggleButton.css` & `anywidget-0.3.0/docs/src/components/Header/ThemeToggleButton.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/src/components/Header/ThemeToggleButton.tsx` & `anywidget-0.3.0/docs/src/components/Header/ThemeToggleButton.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/src/components/LeftSidebar/LeftSidebar.astro` & `anywidget-0.3.0/docs/src/components/LeftSidebar/LeftSidebar.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/src/components/PageContent/PageContent.astro` & `anywidget-0.3.0/docs/src/components/PageContent/PageContent.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/src/components/RightSidebar/MoreMenu.astro` & `anywidget-0.3.0/docs/src/components/RightSidebar/MoreMenu.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/src/components/RightSidebar/RightSidebar.astro` & `anywidget-0.3.0/docs/src/components/RightSidebar/RightSidebar.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/src/components/RightSidebar/TableOfContents.tsx` & `anywidget-0.3.0/docs/src/components/RightSidebar/TableOfContents.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/src/components/examples/Counter.astro` & `anywidget-0.3.0/docs/src/components/examples/Counter.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/src/layouts/MainLayout.astro` & `anywidget-0.3.0/docs/src/layouts/MainLayout.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/src/layouts/SplashLayout.astro` & `anywidget-0.3.0/docs/src/layouts/SplashLayout.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/src/pages/blog/anywidget-02.md` & `anywidget-0.3.0/docs/src/pages/blog/anywidget-02.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 }
 ---
 
 _TL;DR: **anywidget** v0.2 brings modern web development to Jupyter. You can now
 use a **file path** to enable **anywidget**'s integrated Hot Module Replacement (HMR):_
 
 ```sh
-pip install --upgrade anywidget
+pip install --upgrade "anywidget[dev]"
 ```
 
 ```python
 import pathlib
 import anywidget
 import traitlets
 
@@ -189,12 +189,12 @@
 
 
 ## Getting Started
 
 To start using **anywidget** v0.2, upgrade your package using pip:
 
 ```sh
-pip install --upgrade anywidget
+pip install --upgrade "anywidget[dev]"
 ```
 
 I encourage you to explore the new features in **anywidget** v0.2 and experience the
 modern web development practices it brings to the Jupyter ecosystem. Happy coding!
```

### Comparing `anywidget-0.2.4/docs/src/pages/blog/introducing-anywidget.mdx` & `anywidget-0.3.0/docs/src/pages/blog/introducing-anywidget.mdx`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/src/pages/en/bundling.md` & `anywidget-0.3.0/docs/src/pages/en/bundling.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/src/pages/en/getting-started.mdx` & `anywidget-0.3.0/docs/src/pages/en/getting-started.mdx`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 - Prototype **within** `.ipynb` or `.py` files
 - Run in **Jupyter**, **JupyterLab**, **Google Colab**, **VSCode**, and more
 - Develop (optionally) with [Vite](https://vitejs.dev/) for **instant HMR**
 
 ## Example
 
 ```
-pip install anywidget
+pip install "anywidget[dev]"
 ```
 
 ```python
 import anywidget
 import traitlets
 
 class CounterWidget(anywidget.AnyWidget):
```

### Comparing `anywidget-0.2.4/docs/src/pages/en/jupyter-widgets-the-good-parts.md` & `anywidget-0.3.0/docs/src/pages/en/jupyter-widgets-the-good-parts.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/src/pages/en/notebooks/counter.ipynb` & `anywidget-0.3.0/docs/src/pages/en/notebooks/counter.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/src/styles/index.css` & `anywidget-0.3.0/docs/src/styles/index.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/docs/src/styles/theme.css` & `anywidget-0.3.0/docs/src/styles/theme.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/examples/Counter.ipynb` & `anywidget-0.3.0/examples/Counter.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/examples/minimal_example.ipynb` & `anywidget-0.3.0/examples/minimal_example.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/packages/anywidget/CHANGELOG.md` & `anywidget-0.3.0/packages/anywidget/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # anywidget
 
+## 0.3.0
+
+### Minor Changes
+
+- fix: replace deprecated `ipykernel.comm.Comm` with `comm` module ([#119](https://github.com/manzt/anywidget/pull/119))
+
+### Patch Changes
+
+- fix: revert `watchfiles` to optional-dependency ([#118](https://github.com/manzt/anywidget/pull/118))
+
 ## 0.2.4
 
 ### Patch Changes
 
 - fix: add `watchfiles` as a direct dependency ([#116](https://github.com/manzt/anywidget/pull/116))
 
 ## 0.2.3
```

### Comparing `anywidget-0.2.4/packages/anywidget/build.mjs` & `anywidget-0.3.0/packages/anywidget/build.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/packages/anywidget/package.json` & `anywidget-0.3.0/packages/anywidget/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'version'": "'0.3.0'"}*

```diff
@@ -38,9 +38,9 @@
     "name": "anywidget",
     "publishConfig": {
         "main": "dist/index.js"
     },
     "scripts": {
         "build": "node build.mjs"
     },
-    "version": "0.2.4"
+    "version": "0.3.0"
 }
```

### Comparing `anywidget-0.2.4/packages/anywidget/src/widget.js` & `anywidget-0.3.0/packages/anywidget/src/widget.js`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/tests/test_descriptor.py` & `anywidget-0.3.0/tests/test_descriptor.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/tests/test_file_contents.py` & `anywidget-0.3.0/tests/test_file_contents.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/tests/test_utils.py` & `anywidget-0.3.0/tests/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,7 +116,22 @@
     site_packages.mkdir()
     bar = site_packages / "bar.txt"
     bar.write_text("bar")
 
     file_contents = try_file_contents(bar)
     assert isinstance(file_contents, FileContents)
     assert file_contents._background_thread is None
+
+
+def test_try_file_contents_warns(
+    monkeypatch: pytest.MonkeyPatch, tmp_path: pathlib.Path
+):
+    monkeypatch.setitem(sys.modules, "watchfiles", None)
+
+    foo = tmp_path / "foo.txt"
+    foo.write_text("foo")
+
+    with pytest.warns(UserWarning, match="anywidget:"):
+        file_contents = try_file_contents(foo)
+
+    assert isinstance(file_contents, FileContents)
+    assert file_contents._background_thread is None
```

### Comparing `anywidget-0.2.4/tests/test_widget.py` & `anywidget-0.3.0/tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/LICENSE` & `anywidget-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.4/README.md` & `anywidget-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 > **Warning**: **anywidget** is new and under active development. It is not yet
 > ready for production as APIs are subject to change.
 
 **anywidget** is available on [PyPI](https://pypi.org/project/anywidget/) and
 may be installed with `pip`:
 
 ```bash
-pip install anywidget
+pip install "anywidget[dev]"
 ```
 
 It is also available on
 [conda-forge](https://anaconda.org/conda-forge/anywidget). If you have
 [Anaconda](https://www.anaconda.com/distribution/#download-section) or
 [Miniconda](https://docs.conda.io/en/latest/miniconda.html) installed on your
 computer, you can install **anywidget** with the following command:
```

### Comparing `anywidget-0.2.4/pyproject.toml` & `anywidget-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,27 +13,27 @@
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
     "ipywidgets>=7.6.0",
     "importlib-metadata ; python_version < '3.8'",
     "typing-extensions>=4.2.0",
     "psygnal>=0.8.1",
-    "watchfiles>=0.18.0",
 ]
 
 [project.optional-dependencies]
 test = [
     "black[jupyter]",
     "pydantic",
     "pytest",
     "pytest-cov",
     "ruff",
 ]
 dev = [
-    "ipykernel",
+    "comm>=0.1.0",
+    "watchfiles>=0.18.0",
 ]
 
 [project.urls]
 homepage = "https://github.com/manzt/anywidget"
 
 [tool.hatch.build.targets.wheel.shared-data]
 "anywidget/nbextension" = "share/jupyter/nbextensions/anywidget"
@@ -144,9 +144,9 @@
 
 [[tool.mypy.overrides]]
 module = "anywidget.widget"  # makes heavy use of traitlets, which is not typed
 disallow_untyped_calls = false
 
 [[tool.mypy.overrides]]
 # this might be missing in pre-commit, but they aren't typed anyway
-module = ["ipywidgets", "traitlets.*", "ipykernel.*", "IPython.*"]
+module = ["ipywidgets", "traitlets.*", "comm", "IPython.*"]
 ignore_missing_imports = true
```

### Comparing `anywidget-0.2.4/PKG-INFO` & `anywidget-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: anywidget
-Version: 0.2.4
+Version: 0.3.0
 Summary: custom jupyter widgets made easy
 Project-URL: homepage, https://github.com/manzt/anywidget
 Author-email: Trevor Manz <trevor.j.manz@gmail.com>
 License: MIT
 License-File: LICENSE
 Requires-Python: >=3.7
 Requires-Dist: importlib-metadata; python_version < '3.8'
 Requires-Dist: ipywidgets>=7.6.0
 Requires-Dist: psygnal>=0.8.1
 Requires-Dist: typing-extensions>=4.2.0
-Requires-Dist: watchfiles>=0.18.0
 Provides-Extra: dev
-Requires-Dist: ipykernel; extra == 'dev'
+Requires-Dist: comm>=0.1.0; extra == 'dev'
+Requires-Dist: watchfiles>=0.18.0; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: black[jupyter]; extra == 'test'
 Requires-Dist: pydantic; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: ruff; extra == 'test'
 Description-Content-Type: text/markdown
@@ -45,15 +45,15 @@
 > **Warning**: **anywidget** is new and under active development. It is not yet
 > ready for production as APIs are subject to change.
 
 **anywidget** is available on [PyPI](https://pypi.org/project/anywidget/) and
 may be installed with `pip`:
 
 ```bash
-pip install anywidget
+pip install "anywidget[dev]"
 ```
 
 It is also available on
 [conda-forge](https://anaconda.org/conda-forge/anywidget). If you have
 [Anaconda](https://www.anaconda.com/distribution/#download-section) or
 [Miniconda](https://docs.conda.io/en/latest/miniconda.html) installed on your
 computer, you can install **anywidget** with the following command:
```

