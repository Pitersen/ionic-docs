import Playground from '@site/src/components/global/Playground';

import javascript from './javascript.md';
import vue from './vue.md';

import react_main_tsx from './react/main_tsx.md';
import react_main_css from './react/main_css.md';

import angular_app_component_css from './angular/app_component_css.md';
import angular_app_component_html from './angular/app_component_html.md';

<Playground
  code={{
    javascript,
    vue,
    react: {
      files: {
        'src/main.tsx': react_main_tsx,
        'src/main.css': react_main_css,
      },
    },
    angular: {
      files: {
        'src/app/app.component.html': angular_app_component_html,
        'src/app/app.component.css': angular_app_component_css,
      },
    },
  }}
  src="usage/modal/custom-dialogs/demo.html"
  devicePreview
/>
