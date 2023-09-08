---
hide:
  - navigation
---

# Style Guidelines

The purpose of this site is to create a consistent set of very basic conventions used in software development projects at the Blackland Center. We will primarily stick to the language style guildelines, which will be linked in this webpage.

## Repositories

* Repository names should be all lowercase and separate words with a dash (-).
* If the repository should be categoried in some way, prefix your name with this. Examples:
	* We have several projects with TSSWCB. Name in the format: `tsswcb-project-name`
	* If the project is an internal tool, name in the format: `utilities-project-name`
* Repositories should have a `README.md` file containing a brief explanation of the project and build instructions
* For **public** SWAT tools and interfaces, join our [SWAT Model Github](https://github.com/swat-model) organization instead.

## Tabs and spacing

Please adjust your editor to use tabs and not spaces. Tab length should be 4. Some official language style guidelines may mention spaces are preferred: please overrule this for our purposes; tabs are much preferred for all languages.

## .NET C\#

Please follow [Microsoft's .NET naming guidelines](https://learn.microsoft.com/en-us/dotnet/standard/design-guidelines/naming-guidelines) as much as possible. This is just a general rule as there are always exceptions and we do not expect you to memorize every detail. Below are some notable exceptions and suggestions:

* **SWAT variable names** - the SWAT model uses shorthand names for its input and output variables. In older coding projects referencing these inputs/outputs, these names as well as other acronyms were written in UPPERCASE. This practice should only continue in legacy projects. For all new projects, please adhere to the following conventions:
	* Only capitalize the first letter, e.g., `Hru` and not `HRU` or `hru`
	* Underscores while generally not preferred, may be left intact if it matches the name of a SWAT variable, e.g. `Crop_yld` and not `CropYld`, `Crop_Yld`, or `Cropyld`
* **Project names and name spaces** - in general it is preferred to have a common prefix to your project name (e.g. SWAT or HAWQS, written as Swat and Hawqs respectively). Separate words with a period, and only capitalize the first letter of acronyms (historically, this captilization is not always followed in old projects; please adopt going forward). If your solution has multiple projects, name them by function, e.g., `Hawqs.Web`, `Hawqs.Business`, `Hawqs.Data`. If you have a single project but it is part of a common model or entity, prefix with this common word, e.g., `Swat.Conferences` or `Swat.Website`.

## JavaScript / TypeScript / Vue.js

Most JavaScript projects utilize Vue.js. TypeScript is optional, but recommended for larger projects. In general, follow the style guidelines of Vue.js.

### Conventions ###

* Variable and function names should be camel case, e.g., `someVariableName`
* Vue.js component and view (.vue) file names should capitalize the first letter, e.g., `GridView.vue`, while other .js/.ts files should be camel case, starting with a lowercase first letter, e.g. `projectStore.ts`

### Common Packages ###

* Connect to APIs using [axios](https://axios-http.com/docs/intro)
	* Use async/await style instead of .then().finally() method style
* [Vuetify component framework](https://vuetifyjs.com/en/)
	* Vue 2 projects all used [BootstrapVue](https://bootstrap-vue.org/). There is an [alpha version](https://github.com/bootstrap-vue-next/bootstrap-vue-next) for Vue 3 / Bootstrap 5, but Vuetify is preferred at this time due to its immaturity.
	* For simpler applications, you do not need to use a component framework.
* [Font Awesome Icon Package](https://origin.fontawesome.com/)

## Python ##

* Variable and function names should be lowercase and words separated by an underscore (_).


