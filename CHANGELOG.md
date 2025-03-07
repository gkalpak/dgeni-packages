# Changelog

# 0.29.2 2 September 2021

## Bug Fixes

- **base**:
  - improve layout of checkAnchorLinks messages
    [4e5c3e4](https://github.com/angular/angular.js/commit/4e5c3e4)
  - display doc locations even if they are 0
    [a390fbf](https://github.com/angular/angular.js/commit/a390fbf)
 - **ngdoc**: link filter - correctly handle missing title
    [affb49e](https://github.com/angular/angular.js/commit/affb49e)

## New Features
- **jsdoc**: add support for parsing ES2017 syntax
  [974173d](https://github.com/angular/angular.js/commit/974173d)

# 0.29.1 27 April 2021

## Bug Fixes
- **git:** use the package version if no tag satisfies
  ([c72834](https://github.com/angular/angular.js/commit/c72834c853cb4d3756d5f4d64f2637af30f2465f))


## New Features
- **git:** add `getPreviousVersions.versionMatcher`
  ([571659](https://github.com/angular/angular.js/commit/5716591f724087a16605d791fcfd44179607568c))


# 0.29.0 6 April 2021


## Bug Fixes
- **nunjucks:** do not fail on undefined value by default
  ([cefb9e](https://github.com/angular/angular.js/commit/cefb9e0c7ad8fe82a2542758d1719d5d93868757))


## New Features

- **jsdoc:**
  - add support for version tag
    ([0fe303](https://github.com/angular/angular.js/commit/0fe303e593fe04769d6cec958126082e6a541e55))
  - add support for more jsdoc tags
    ([169c41](https://github.com/angular/angular.js/commit/169c41a1238dbdf06c29424026b940c21cab7fd5))
- **jsdoc,nunjucks:** update espree and nunjucks packages
  ([c2a463](https://github.com/angular/angular.js/commit/c2a463dfc0fdc322c893e72548aede41103a1719))


# 0.28.4 27 June 2020

## Bug Fixes
- **typescript**: render type initializations
  ([abfdf5](https://github.com/angular/angular.js/commit/abfdf5a57b71e0de3d3092a316839b8ae626c696),
  [#290](https://github.com/angular/dgeni-packages/issues/290))


# 0.28.3 12 February 2020

## Bug Fixes
- **base:** ensure writeFile() actually writes files to disk
  ([eda95f](https://github.com/angular/angular.js/commit/eda95f7f966d8d8257ebcbcbabf4b7a3f46075aa),
  [#287](https://github.com/angular/dgeni-packages/issues/287))


# 0.28.2 21 November 2019

## Bug Fixes
- **git:** use correct shell execution status property
  ([ed275635a](https://github.com/angular/angular.js/commit/ed275635adc5f2a6b2b82b26b3150fdb8aaddc36))


# 0.28.1 2 April 2019

* Chore release - updating dependencies and switching from `node-html-encoder` to `htmlencode`

# 0.28.0 12 July 2019

## Bug Fixes
- **git:** remove `shelljs` dependency
  ([18a1c0](https://github.com/angular/angular.js/commit/18a1c0b0692c05d43126150f1d8e284850ea2da3))
- **nunjucks:** upgrade `marked` to avoid vulnerability
  ([16ceb9](https://github.com/angular/angular.js/commit/16ceb9c9bc9aac168f82db977a9e380fb20b815a),
  [#280](https://github.com/angular/dgeni-packages/issues/280))

## Breaking Changes

### **nunjucks** due to:
  - **[16ceb9](https://github.com/angular/dgeni-packages/commit/16ceb9c9bc9aac168f82db977a9e380fb20b815a)**: upgrade `marked` to avoid vulnerability

There are a few relevant breaking changes with this latest version of `marked`.
This only affects usage of the `renderMarkdown()` service and the `marked`
nunjucks filter. Take a look through the
[marked release notes](https://github.com/markedjs/marked/releases) and
check if this affects you.


# 0.27.4 1 July 2019

## Fixes

fix(post-process-html): ensure files are correctly published to npm   15ecab0631


# 0.27.4 1 July 2019

# Features

feat(post-process-html): add new post-process-package    9798f22 & aac5e8e8


# 0.27.3 2 April 2019

* Chore release - updating dependencies


# 0.27.2 14 March 2019

* Chore release - updating dependencies


# 0.27.1 29 December 2018

## Fixes

* **typescript**: implemented method overload should have simple id and aliases	  398f35da3


# 0.27.0 17 December 2018

## Dependencies

* update to latest nunjucks package   c84134b
* update to latest TS version (3.2)   610d19b
* update to latest canonical-path     2b8e51e

## BREAKING CHANGES

The upgrade to TypeScript 3.2.2 has brought a couple of minor breaking changes:

* the algorithm that truncates long types has changed.
Types are now truncated at the AST node level, so are more syntactically
accurate. Also some long types are no longer truncated.
* the order of exports from a module has changed.
Previously the exports were listed in the order that they appear in the sourcefile.
Now classes appear to be listed before functions.

# 0.26.12 23 October 2018

## Fixes

* **typescript**: use correct optional parameter type	148bc949


# 0.26.11 23 October 2018

## Features

* **typescript**: allow specifying type format flags for api-doc-types 5d90fd9f31541


# 0.26.10 21 September 2018

## Fixes

* **nunjucks**: disable autoescape for marked tag	067f74c5


# 0.26.9 2 September 2018

## Fixes

* **typescript**: empty node description if first leading comment is single line trivia   5c8c4ac


# 0.26.8 31 August 2018

## Features

* **typescript**: improve declaration type text rendering	da3323f7

# 0.26.7 29 August 2018

## Fixes

* **typescript**: do not throw if node does not have any comment  8f6cb87

# 0.26.6 28 August 2018

## Features

* **typescript**: add option to disable leading comment concatenation	bd748bb2

# 0.26.5 21 August 2018

## Fixes

* **jsdoc**: support void/self-closing/custom HTML tags	   2407ee68

# 0.26.4 20 August 2018

## Fixes

* **typescript**: invalid path delimiter for triple slash type directives in windows	  9964b0a1

# 0.26.3 16 August 2018

## Fixes

* **typescript**:
 - handle special case for triple slash reference types directives	b22dab5b


# 0.26.2 16 May 2018

## Features

* **typescript**:
 - include simple name in aliases of members  1d952fd5


# 0.26.1 11 May 2018

## Fixes

* **typescript**:
 - correctly compute the type of "const" docs	 17078928


# 0.26.0 2 March 2018

## Features

* **typescript**:
 - add `isAbstract` properties to classes and members	315b6ceb
 - use TypeScript v2.7 to parse the TS source files	85ffe3a0

## BREAKING CHANGES:

The new version of TypeScript has better handling for specially named members such
as `__constructor` and `__call`. To support this the TypeScript API introduced a new
type `__String` for holding escaped versions of these strings.

This makes is much safer in case a member name collided, but it also introduces a
breaking change to the TypeScript AST public interface.

This will not affect developers using the `typescript` package unless they are trying
to interact with the TS AST directly, or they were expected to interact with escaped forms
of special names, such as `__esModule`, which is `___esModule` in its escaped form.


# 0.25.0 28 February 2018

## Fixes

* **typescript**:
  - remove `namespacesToInclude` feature  6a893df3
  - give `path` and `outputPath` initial values c5f3049f

## Breaking Change

The `namespacesToInclude` service has been removed from
the package. Now when rendering types full qualified names are
always rendered and no namespaces are stripped.

If you relied on this then you should implement a processor to
search for these rendered types and strip them.


# 0.24.3 25 February 2018

## Features

* **typescript**: expose `defaultValue` information on ParameterDocs	ba8f57fa


# 0.24.2 24 Febrary 2018

## Features
* **typescript**:
  - expose `isOptional` information on ParameterDocs  39ad2feb
  - create `BaseApiDoc` class                         9586f881

## Fixes
* **typescript**:
  - `ParameterDoc` is a type of `BaseApiDoc`, not `ExportDoc` d00b3ed2
  - only use unix style line endings when rendering code      ef1f83c9


# 0.24.1 7 February 2018

## Fixes
* **jsdoc**: braces in the description are not jsdoc types	35763aafa
* **typescript**: fallback to decorators from set accessor	3a4e56855
* **jsdoc**: handle import statements in code name matching	5db8fc90f


# 0.24.0 26 January 2018

## Fixes
* **typescript**: align default path and id templates	0ff52e2b
* **typescript**: do not encode anchors for member API docs	7cad9780
* **base**: checkAnchorLinksProcessor now copes with encoded chars	f7f6f589

## BREAKING CHANGE

Anchors to member API docs, whch are accessed via `doc.anchor` are no
longer URL encoded. You should do this in your template if that is required.

* Before: `<a href="{$ doc.anchor $}">...</a>`
* After: `<a href="{$ doc.anchor | urlencode $}">...</a>`


# 0.23.0 17 January 2018

## Fixes

* **typescript**:
  - show proper name for aliased exports	f7034143

## Features

* **jsdoc**:
  - improve support for named exports in the codeName service	45c28b61
* **typescript**:
  - merge `@param` descriptions into `ParameterDoc`s	af7f5213
  - process parameters as docs	4d04d8f9
  - move helpers to ModuleDoc to simplify API doc constructors	a776355c

## BREAKING CHANGE

The constructor signatures for API API docs have changed. You no longer need to pass
the `basePath`, `namespacesToInclude` or `typeChecker` to any API doc constructor
except for the `ModuleDoc`. All API docs now get hold of these values from their
containing `ModuleDoc`.

Generally this should not affect users of dgeni-packages since it is not expected
that API doc classes should be instantiated directly.


# 0.22.1 23 November 2017

## Fixes

* **typescript**: remove comments from re-rendered code	0be17b9a

# 0.22.0 9 October 2017

## Fixes

* **typescript**: handle property accessors correctly	f72b69e5f

## BREAKING CHANGE

To support the handling of get and set accessors, there are new docTypes
"get-accessor-info" and "set-accessor-info", which need templates.

# 0.21.6 9 October 2017

## Reverts

* **typescript**: handle property accessors correctly	a4be78add

This change introduced a breaking change, which is that there are new docTypes
"get-accessor-info" and "set-accessor-info", which need templates.

# 0.21.5 8 October 2017

## Fixes

* **typescript**: handle property accessors correctly	75fafcf7

# 0.21.4 28 September 2017

## Features

* **typescript**:
  - add isReadonly flag to member docs	62bc5333
  - include typeParameters in type-alias docs	51d81496

## Fixes

* **typescript**: show both type and initializer on parameters	d677e72a


# 0.21.3 22 September 2017

## Features

* **typescript**: track descendants of inherited classes	b64e8519

# 0.21.2 11 September 2017

## Fixes

* **typescript**: do not render comments in decorator arguments	7cfd8021

## Chores

* upgrade to TypeScript 2.4	1d64fcc7

# 0.21.1 4 September 2017

## Features

* **typescript**: support overloaded constructors	ca69213d

## Bug Fixes

* **typescript**: fix possibly null references	463ef5cf

# 0.21.0 4 September 2017

## Features
* **typescript**: reference `extands` and `implements` ancestor info	d7c29603

## BREAKING CHANGES:

Previously, the `doc.implementsClauses` and `doc.extendsClauses` were arrays
of strings, describing the text of the clause.

Now, these properties are of type `HeritageInfo`:

```typescript
class HeritageInfo {
  symbol: Symbol | undefined;
  doc: ClassLikeExportDoc | undefined;
  type: ExpressionWithTypeArguments;
  text: string;
}
```

where the `text` property holds the value that was previously provided.

You need to change your code/templates to access the text of the heritage
clause from:

```
{% for clause in doc.extendsClauses %}{$ clause $}{% endfor %}
```

to:

```
{% for clause in doc.extendsClauses %}{$ clause.text $}{% endfor %}
```

# 0.20.1 16 August 2017

## Features
* **jsdoc**: add propertyof jsdoc tag	6712e544

## Fixes

* **dgeni**: ensure that dgeni self documenting config works	8052e9e6


# 0.20.0 27 July 2017

This is the full release of 0.20.0 - the list of changes below includes all the beta and release candidate changes.

## Features

- **base:** allow checkAnchorLinks to abort processing	eee3e7b1
- **typescript:**
  - group function/method overloads together	2155b5ac
  - provide isCallMember and isNewMember options
  - split out heritage into extendsClauses and implementsClauses
  - add `realFilePath`/`realProjectRelativePath` to `FileInfo`	c7d1b54c

## Performance Improvements
- **nunjucks:** upgrade to v3 and enable caching of templates

## Bug Fixes

- **ngdoc:** pass doc object to createDocMessage	fe98a849	Nick Horvath
- **typescript:**
  - add type parameters to function export docs	c2c29270
  - remove duplicate overload from abstract API doc members	f2c481d1
  - support startingLine and endingLine properties	32698f30
  - include specified namespaces in types	dbe99f7b
  - allow decorators to not be call expressions	e41a392a
  - implement the CompilerHost.readFile method	4d667ff2
  - CustomCompilerHost.fileExists should not second guess extensions and base dir	b7b11164
  - compile files in folders that have file-like names	ee10b835
  - paths should be case sensitive	5238302b
  -	compile files in folders that have file-like names
  - paths to imports are case sensitive
  - group overloaded exported functions in a single doc
  - do not assume that members prefixed with `_` are private
- **base:** checkAnchorLinks should match URL encoded chars

## Breaking Changes

Previously to 0.20.0 the service where you registered namespaces not to strip
was called `ignoreTypeScriptNamespaces` and took an array of regular expressions.

Now this service is called `namespacesToInclude`, which better reflects its
purpose. Also it is now an array of strings, since there was little benefit in it
being a regular expression.

<hr>

The typescript package has been completely rewritten in TypeScript. One benefit of this is that
typings should be available for the API doc types in your own projects.

Along the way there are some changes to the properties that are attached to the API docs that are
generated. Here is a list of the things that might affect you:

* Members starting with `_` are no longer considered private. You should filter them out in a
custom processor if you do not want them to appear in the docs.
* API docs that have a type, e.g. functions, constants, type aliases, etc used to have a property called
`returnType` but that did not make sense for non-functions. This property is renamed to `type`.
* API docs that have heritage, e.g. classes and interfaces, used to have a property called `heritage`,
which was a string representation containing both "implements" and "extends" clauses. These have now
been split into two properties `implementsClauses` and `extendsClauses`, which each contain an array
of strings.


# 0.20.0-rc.6  14 July 2017

## Bug Fixes

**typescript:** add type parameters to function export docs	c2c29270


# 0.20.0-rc.5  13 July 2017

## Bug Fixes

**typescript:** remove duplicate overload from abstract API doc members	f2c481d1
**ngdoc:** pass doc object to createDocMessage	fe98a849	Nick Horvath


# 0.20.0-rc.4  13 July 2017

## Bug Fixes

**typescript:** support startingLine and endingLine properties	32698f30


# 0.20.0-rc.3  12 July 2017

## Features

**typescript:** group function/method overloads together	2155b5ac

## Bug Fixes

**typescript:** include specified namespaces in types	dbe99f7b

## Breaking Changes

Previously to 0.20.0 the service where you registered namespaces not to strip
was called `ignoreTypeScriptNamespaces` and took an array of regular expressions.

Now this service is called `namespacesToInclude`, which better reflects its
purpose. Also it is now an array of strings, since there was little benefit in it
being a regular expression.


# 0.20.0-rc.2  10 July 2017

## Bug Fixes

- **typescript:** allow decorators to not be call expressions	e41a392a


# 0.20.0-rc.1  6 July 2017

## Bug Fixes

- **typescript:** implement the CompilerHost.readFile method	4d667ff2

## Features

- **base:** allow checkAnchorLinks to abort processing	eee3e7b1


# 0.20.0-beta.5  2 July 2017

## Bug Fixes

- **typescript:** CustomCompilerHost.fileExists should not second guess extensions and base dir	b7b11164


# 0.20.0-beta.4  1 July 2017

## Bug Fixes

- **typescript:**
  - compile files in folders that have file-like names	ee10b835
  - paths should be case sensitive	5238302b

# 0.20.0-beta.3  30 June 2017

## Bug Fixes

-	**typescript:** compile files in folders that have file-like names

# 0.20.0-beta.2  30 June 2017

## Bug Fixes

- **typescript:** paths to imports are case sensitive

# 0.20.0-beta.1  29 June 2017

## BREAKING CHANGES

The typescript package has been completely rewritten in TypeScript. One benefit of this is that
typings should be available for the API doc types in your own projects.

Along the way there are some changes to the properties that are attached to the API docs that are
generated. Here is a list of the things that might affect you:

* Members starting with `_` are no longer considered private. You should filter them out in a
custom processor if you do not want them to appear in the docs.
* API docs that have a type, e.g. functions, constants, type aliases, etc used to have a property called
`returnType` but that did not make sense for non-functions. This property is renamed to `type`.
* API docs that have heritage, e.g. classes and interfaces, used to have a property called `heritage`,
which was a string representation containing both "implements" and "extends" clauses. These have now
been split into two properties `implementsClauses` and `extendsClauses`, which each contain an array
of strings.

## Bug Fixes
- **typescript:**
  - group overloaded exported functions in a single doc
  - do not assume that members prefixed with `_` are private
- **base:** checkAnchorLinks should match URL encoded chars


## New Features
- **typescript:**
  - provide isCallMember and isNewMember options
  - split out heritage into extendsClauses and implementsClauses

## Performance Improvements
- **nunjucks:** upgrade to v3 and enable caching of templates


# 0.19.1 26 May 2017

* fix(typescript): capture static members correctly	0e41fae7


# 0.19.0 3 May 2017

- feat(typescript): upgrade to TypeScript 2.2.1	0f48e866

## Breaking Changes

The upgrade to TypeScript v2 may well break projects that are generating docs
based on a TypeScript v1 application.

# 0.18.0 30 April 2017

- fix(typescript): remove `index` from the end of module ids and names
  ([e6109f57](https://github.com/angular/dgeni-packages/commit/e6109f57266df1edde37071e985d58cda76c1bf1))

## Breaking Changes

  This has a possible breaking change if users were depending upon a module at `/some/folder/index.ts`
  having a name of `index` and an id of `some/folder/index`.

# 0.17.2 26 April 2017

## Bug Fixes

- **jsdoc:** reset backTickParserAdapter correctly
  ([a82ea9ab](https://github.com/angular/dgeni-packages/commit/a82ea9ab24d718d7c90b4d8766f3308e28019fec))


# 0.17.1 17 March 2017

## Bug Fixes
- **typescript:** ensure all modules have relative filepaths
  ([434233](https://github.com/angular/dgeni-packages/commit/43423313e246e07a002d2410182d1157b206dbc7))


# 0.17.0 17 March 2017

## Bug Fixes
- **jsdoc:** do not parse for tags within HTML blocks
  ([451d84](https://github.com/angular/dgeni-packages/commit/451d84a0d0e4bdfd675bced61dd3f2e9cef533a0))

## Breaking Changes

### **jsdoc** due to:
  - **[451d84](https://github.com/angular/dgeni-packages/commit/451d84a0d0e4bdfd675bced61dd3f2e9cef533a0)**: do not parse for tags within HTML blocks

    Tags inside HTML blocks are no longer parsed by default.
    If you wish this to enable this then you can modify the
    `parseTagsProcessor.parserAdapters` array from a config block:

    ```
    somePackage.config(function(parseTagsProcessor, backtickParserAdapter) {
      parseTagsProcessor.parserAdapters = [backtickParserAdapter];
    });
    ```


# 0.16.10 7 March 2017

* REVERT: feat(typescript): link `class` docs to inherited class docs	cf8b7444

# 0.16.9 6 March 2017

* feat(typescript): link `class` docs to inherited class docs	cf8b7444


# 0.16.8 20 February 2017

* fix(typescript): correctly extract the type definition from type aliases	573111ea


# 0.16.7 15 February 2017

Upgrades to dgeni 0.4.7 which correctly exports the mock logger for testing.

* fix(typescript): the processors actually rely upon jsdoc pseudo-processors	f5162131

# 0.16.6  13 February 2017

* fix(typescript): support symbols of type ValueModule	ffce6227


# 0.16.5  14 January 2017

* chore(package): relax node version dependency 8ad91e57

# 0.16.4  23 December 2016

* chore(package): add missing mkdirp dependency	0a2c2e9f

# 0.16.3  21 December 2016

* chore(package): relax yarn version dependency	0f875b0d

# 0.16.2  16 December 2016

*	refactor(*): remove Q and use native Promise 	d782698d

This fix removes the q and q-io dependencies, since q-io was causing Array.find
to be shimmed incorrectly.

# 0.16.1  13 December 2016

* fix(base/services): split node-html-encoder require and instantiation over two lines   96cb8139e8876150b5a6ce08f2c5eef7fbd791f6


## v0.16.0 13 September 2016

* fix(readTypeScriptModules): don't concatenate multiple declarations		fb22bac5

### BREAKING CHANGES

Previously, if there were multiple declarations for an exported symbol,
then the docs for those declarations were simply joined together with
newlines.

Now only the first declaration (or the valueDeclaration if there is one)
is used in an export doc.

If you needed the content for the other declarations then you can still
access them via a call like `getContent(doc.additionalDeclarations[i])`.

## v0.15.2 9 September 2016

* feat(typescript/readTypeScriptModules): hide private Typescript members  8a1277de


## v0.15.1 6 September 2016

* fix(git): allow for git URLs that start with `git+https:`	c27a324d
* doc(readme_fr_FR) : update readme in french	 da7f6b3c
* fix(ngdocs): use `import` syntax for macros		9a69a096
* fix(nunjucks): explicitly set autoescaping to off		54e20018
* fix(nunjucks): warnings for upgraded API, add error check		e339b7d8
* chore(package.json) update nunjucks to 2.4.2	01108e4e

### BREAKING CHANGES

The update to `nunjucks` 2.4.2 has changed how macros are used. Now you must import them rather than
just including them in a template. See http://mozilla.github.io/nunjucks/templating.html#import for
more detail on the syntax.

Before:

```
{% include "lib/macros.html" -%}
{$ functionSyntax(doc) $}
```

Now:

```
{% import "lib/macros.html" as lib -%}
{$ lib.functionSyntax(doc) $}
```

The templates provided by this project (in particular those in the `ngdocs` package) have been updated
but if your project uses macros in its own templates then these will need updating too.

## v0.14.0 4 July 2016

Major update of dependencies to latest.

* chore(package.json): update lodash to 4.13.1	f082551
* chore(package.json): update lodash to 3.x	a37d110
* chore(package.json): update q-io to 1.13.2	79819fa
* chore(package.json): update q to 1.4.1	9bb7490
* chore(package.json): update semver to 5.2.0	5bfdbba
* chore(package.json): update shelljs to 0.7.0	5480c55
* chore(package.json): removed unused packages	1546b8e
* chore(package.json): update glob to 7.0.5	5208f8a
* chore(package.json): update change-case to 3.0.0	7fcc9c7
* chore(package.json): update minimatch to 3.0.2	8f57d2c


### BREAKING CHANGES

The `nunjucks` package rendering filter `sentenceCase` now capitalizes
the first letter of the sentence. If you relied on the previous behaviour
then you should use the `noCase` filter instead.


## v0.13.1 1 July 2016

* fix(typescript/readTypeScriptModules): `getReturnType` should cope with computed initializers	823d3f9e
* fix(ngdoc/macros): use `type.name` to display the directive parameter types	18193fee


## v0.13.0 12 May 2016

* fix(jsdoc/access): refactor access tags and transforms to allow more configuration	70cd0bea
* fix(typescript/createCompilerHost): fix syntax errors	ae47de91
* refactor(jsdoc/codename): add service, made matchers pluggable	28dc7919
* fix(restrict): Change default from 'A' to 'EA'.	e0e6a501
* fix(jsdoc/extract-tags): don't write properties if tag values are `undefined`	3eade6bc

### BREAKING CHANGES

* Due to 3eade6bc
  Tags that had a value of `undefined` are no longer written to the document.
  If you relied upon such falsy values forcing keys onto the doc, then change
  your tagDefs to return `null` instead.
* Due to e0e6a501
  If you don't provide a value for the `@restrict` tag it now defaults to `EA` rather
  than just `A`. If you want your directives to be only `A` then you must provide a
  `@restrict` tag for them.
* Due to 70cd0bea
  The way that you configure `extractAccessTransform` has changed. If you were creating
  your own access tags then you must use the new API.

  Previously:

  ```
  module.exports = function(accessTagTransform) {
    var name = 'private';

    accessTagTransform.addTag(name);
    accessTagTransform.addValue(name);

    function getValue () {
      return name;
    }

    return {
      name: name,
      docProperty: 'access',
      transforms: [getValue, accessTagTransform]
    };
  };
  ```

  Now:

  ```
  module.exports = function(extractTypeTransform, extractAccessTransform) {
    extractAccessTransform.allowedTags.set('private');
    return {
      name: 'private',
      transforms: [extractTypeTransform, extractAccessTransform]
    };
  };
  ```

## v0.12.0 3 April 2016

### Features

* feat(typescript): add package to parse exports from TypeScript modules	3e07adee
* feat(jsdoc): add support for @access, @private, @protected, @public tags	e87f61f3
* feat(ngdoc): add knownIssues tag and processing	b590d058

### Fixes

* fix(jsdoc): only declare private tagDef once	04b6e08e
* fix(git): allow non-github repository URLs	afc213cc
* fix(examples): don't error if the doc has no content	2944e203
* fix(ngdoc/api.template): use link filter for module link	4f4ab7ef
* fix(code-name): add support for MethodDefinition, ArrowFunctionExpression nodes	cf2c28bf
* fix(git/versionInfo): don't throw error if there is no valid codename	d749314c


## v0.11.1 7 November 2015

* fix(jsdoc/inline-tags): don't conflate successive inline tags when matching  67c2abf5
* feat(jsdoc): add license tag   6f4bb5f7
* feat(docs): improve templates and add npm script for generating docs   3c75243e
* feat(dgeni): compute the full pipeline of processors for each package and add index page   c12cd9ec


## v0.11.0 31 October 2015

**ES6 Support:**

* fix(code-name): update espree, estraverse and add support for ExportDefaultDeclaration  Yair Leviel 080620c2
* fix(jsdoc/jsParser): support parsing ES6 features Peter Bacon Darwin  c14c18ce

**Dgeni self-documentation:**

* feat(docs): initial dgeni doc-gen package Peter Bacon Darwin  603e333e
* feat(docs): initial dgeni doc-gen package Peter Bacon Darwin  8c176e53
* feat(dgeni): add dgeni configuration documentation processing Peter Bacon Darwin  0f4f5dd4

**Links package:**

* feat(links): initial links package, abstracted from the ngdoc package Peter Bacon Darwin  94271a1a

**Start-End Inline Tags**

* feat(inline-tags): allow start-end tags Peter Bacon Darwin  362a3495

**Bug Fixes**

* fix(versionInfo): don't crash if no codename match is found Peter Bacon Darwin  069c7762
* fix(jsdoc) file-readers assignment via concat Matt Fairbrass  c6af7204

## v0.10.19 23 August 2015

* fix(ngdoc/templates): move module installation above description  6f7b0fc3


## v0.10.18 10 July 2015

* fix(jsdoc/private tagdef): assign true to private property if tag is found  640d3da6


## v0.10.17 23 June 2015

* fix(git/api.template): remove weird character in folder name 3ad11ff1


## v0.10.16 22 June 2015

* fix(ngdoc): remove `git` package as a dependency  f0647968
* fix(git/packageInfo): ensure that we return consistent paths on all OSes  4e29bb62


## v0.10.15 21 June 2015

* feat(git): add git information package  81944685
* fix(ngdoc/templates/lib/events): add event params  860dce98
* fix(extractTypeTransform): support record types 32b269aa
* feat(ngdoc/multiElement tag): directives can declare that they support multiElement 41d583f8


## v0.10.14 11th June 2015

 * fix(checkAnchorLinks): add decodeURIComponent call when checking for dangling links d5ed516b
 * feat(ngdoc/getLinkInfo): add option to make links relative 7178e9eb

## v0.10.13 2rd April 2015

* fix(ngdoc/macros.html): use optional property from param rather than type


## v0.10.12 13th March 2015

* chore(packages): update nunjucks to 1.2.0


## v0.10.11 13th March 2015

* fix(jsdoc/extract-type): improve error message e56ea300


## v0.10.10 15th February 2015

* fix(jsdoc/parseTagsProcessor): cope with single line back-ticked code blocks  0d5892d0


## v0.10.9 15th Februrary 2015

* fix(base/trimIndentation): cope with empty text blocks  8cb1bcb8


## v0.10.8 15th December 2014

* fix(base/checkAnchorLinksProcessor): ignore "chrome://..." links    3d5dca46
* fix(nunjucks/firstLine): don't break inline tags when extracting first line    19a642f1


## v0.10.7 18th November 2014

* fix(base/trimIndentation): ensure that lines that start at index zero kill the indentation      434a9b4a
* fix(example/template.js): add functional form of 'use strict'    f909b9c7
* feat(base/readFilesProcessor): accept arrays of include and exclude patterns      696c4c68
* fix(example/template.js): add 'use strict'    a0ceb1e
* fix(ngdoc/$moduleDocs): throw an error if a module is improperly tagged    d6edbffd


## v0.10.6 10th November 2014

* fix(base/resolveUrl) : Handle the path c:\ under Windows       ef23d430
* fix(jsdoc/extractTagsProcessor): remove parameter that was hiding the real variable      ba34f921


## v0.10.5 15th October 2014

* feat(examples/generateProtractorTestsProcessor): allow basePath of test to be specified     2bfb6666


## v0.10.4 15th October 2014

* fix(base/checkAnchorLinks): match links using pathVariants       ff903657
* fix(jsdoc/jsdocFileReader): provide file information in JS parse error     69680361


## v0.10.3 9th October 2014

* fix(ngdoc/directive.template): add `id` to the `Animations` heading    6e9253d6


## v0.10.2 8th October 2014

* feat(examples): allow external example dependencies      ae900e77

## v0.10.1 6th October 2014

Mostly minor refactoring and the new `checkAnchorLinksProcessor`

Thanks to Lucas, Thor and Stéphane.

* refact(base/checkAnchorLinksProcessor): cleaned up the processor     537f6228
* refact(base/extractLinks): rename and also extract id attributes     3ef7b3af
* refact(base/resolveUrl): simplify the code       f393d4ac
* feat(anchors): detect dangling anchors     b9b3ef8c
* refact(base/computePathsProcessor): warn if no path or outputPath template/getter is found       a5b9f536
* refact(jsdoc/jsdocfileReader): move processing into extractJSDocCommentsProcessor     cbcbac23
* feat(jsdoc/extractJSDocComments): add new processor      b1362834
* fix(jsdoc/parseTagsProcessor): don't error if doc has no content      b3da03c3
* feat(ngdoc/templates/base.template): make 'Improve this Doc' lead to appropriate line      55f5f002


## v0.10.0 29th September 2014

Finally, only 4 betas and 7 release candidates and here is 0.10.0. This version is current being
used in production by the angular.js project.

* feat(ngdoc/templates/base.template): prefill 'Improve this Doc' commit msg   eafb1d2f


## v0.10.0-rc.7 26th September 2014

* fix(ngdoc/templates): fix the github URLs     ce548496
* feat(examples/generateExamplesProcessor): allow css-dependencies in examples      10b8278f


## v0.10.0-rc.6 17th September 2014

* feat(examples/index.template.html): add `ng-csp` conditionally     4e173614


## v0.10.0-rc.5 15th September 2014

### Bug fixes - Nunjucks

fix(nunjucks/marked filter): use renderMarkdown service      c82e6a26
fix(nunjucks/marked custom tag): use renderMarkdown service      1ec39d19
feat(nunjucks/renderMarkdown): add new service to allow custom markdown rendering    47ee5ec1

### New features - JSDoc File Reader

* feat(jsdoc/jsdocFileReader): add AST to the fileInfo      998738a7
* refact(jsdoc/jsdocFileReader): use estraverse rather than hacked walk.js      6f8279ce


## v0.10.0-rc.4 12th September 2014

Bug Fixes:

* fix(examples/generateExamplesProcessor): manifest files should be an array of strings    caf321ec
* fix(ngdoc/memberDocs): strip modifier from member name     b0b53ec5


## v0.10.0-rc.3 11th September 2014

Fixes:

* feat(ngdoc/providerDocsProcessor): add missing processor     2ea87c15
* fix(ngdoc/moduleDocsProcessor): add missing var declaration    196c1758

Testing Improvements

* test(ngdoc/getLinkInfo): test missing and URL based links    4170e83f
* refact(ngdoc/moduleDocsProcessor): improve and test error messages     d749563f
* test(base/writeFilesProcessor): test corner cases     fef7a919
* test(nunjucks/filters): add missing tests     13dc8a77
* test(jsdoc/extractTagsProcessor): test corner cases     b8157723
* test(base/readFilesProcessor): add corner case tests      17765d52

## v0.10.0-rc.2 10th September 2014

Bug fix

* fix(examples/generateProtractorTestsProcessor): enable testing 'ng-app-included' examples    46a0c516


## v0.10.0-rc.1 10th September 2014

Minor refactoring

* chore(package.json): fix path to tests in npm scripts     2924a3ac
* chore(package.json): remove pre and post install hooks      6dd05b21
* chore(examples): move tests into source folder      f128fede
* chore(ngdoc): move tests into source folder     b5df9a16
* chore(nunjucks): move tests into source folder      cce54a00
* chore(jsdoc): move tests into source folder     9b337073
* chore(base): move tests into source folder      43b64bbf


## v0.10.0-beta.4 6th September 2014


### Refactorings

#### ComputeIdsProcessor

The major refactoring in this release was to move computation of ids (and aliases, which used to be called
partialIds) into a generic computeIdsProcessor in the base package.  This is then configured (similar to
computePathsProcessor) for each docType that a package introduces.


* fix(ngdoc): fix idTemplate for member docTypes    dbad1945
* fix(examples): add idTemplates for examples docTypes    16086476
* fix(ngdoc/getDocFromAlias): start from scratch if filtering by area fails     f742f5a3
* fix(ngdoc/getLinkInfo): pass through currentDoc when searching for member     039deedf
* refact(computeIdsProcessor): rename partialIds to aliases     00607193
* refact(base/aliasMap): remove unused reference to lodash      3321da6b
* refact(ngdoc): use computeIdProcessor and aliasMap      569312c9
* refact(getPartialNames): rename to getAliases     ee83af87
* feat(ngdoc/getDocFromAlias): add service to find relative docs from alias     bef71895
* refact(base/computeIdProcessor): rename partialIdMap to aliasMap      e336bbc3
* refact(partialIdMap): rename to aliasMap      46075fb3
* feat(base/computeIdsProcessor): add new processor to compute ids based on configuration templates     aeec7e1e
* feat(base/partialIdMap): add new service for storing partial ids      1c3f82ab
* refact(base/computePathsProcessor): always regenerate the maps on $process      4caa96c7
* refact(ngdoc/getAliases): combine getPartialNames and parseCodeName into getAliases     2d3071f0
* refact(ngdoc/getLinkInfo): use getDocFromAlias      0cc9f490
* refact(ngdoc/computeIdProcessor): remove and use base/computeIdsProcessor     e17d808c
* test(jsdoc): disable computeIdsProcessor for test     e303f3c7
* refact(ngdoc/partialNameMap): remove and use aliasMap from base instead    925c01a1
* docs(ngdoc/getDocFromAlias): document the service   167a982b
* fix(base/computeIdsProcessor): improve error messages   88ea6e10
* fix(jsdoc): provide basic getPartialIds function    54dc8118
* refact(jsdoc): update to use computeIdsProcessor    2938a4c5


#### apiDocsProcessor

Also the apiDocsProcessor was broken up. Part of it is now handled by the `computeIdsProcessor` but the rest
was refactored into `membersDocsProcessor` and `moduleDocsProcessor`.

* refact(ngdoc/generateComponentGroupsProcessor): apiDocs is going away      1fbed695
* refact(ngdoc/apiDocsProcessor): remove old processor       c1a2fee0
* refact(ngdoc/moduleDocsProcessor): use getDocFromAlias       fa0408ca
* refact(ngdoc/memberDocsProcessor): use getDocFromAlias       74063d3f
* fix(ngdoc/memberDocsProcessor): test and ensure doc.memberof is a full id      f6b063dd
* fix(ngdoc/moduleDocsProcessor): run after memberDocsProcessor      c3fd9398
* fix(ngdoc/moduleDocsProcessor): better resolve ambiguous module references       b27d8ff7
* test(ngdoc/moduleDocsProcessor): test the processor      3e42370c
* refact(ngdoc): reorganization of processors and services       c7397fa1
* feat(ngdoc/moduleDocsProcessor): extract functionality from apiDocsProcessor     8cd51dc4
* feat(ngdoc/memberDocsProcessor): extract functionality from apiDocsProcessor     c7302275


#### `dgeni.configureInjector` and tests

The a new version of dgeni allowed us access to the injector without having to run `dgeni.generate()`.
This meant that we could have much cleaner tests, where we can let the injector create our services rather than
having to wire them up manually - which was a pain and error prone.

* test(ngdoc/getLinkInfo): use mockPackage for testing      896cad63
* test(ngdoc/getDocFromAlias): test with mockPackage      b819e338
* test(ngdoc/mockPackage): add mock Package for testing     659e8d09
* test(ngdoc/filterNgDocsProcessor): use mockPackage and injector     2eea5026
* test(ngdoc/generateComponentGroups): use mockPackage and injector     13da2040
* test(jsdoc): use mockPackage      9d08564b
* test(base/computePathsProcessor): get mockLog from injector     b154d5a2
* test(base/computeIdsProcessor): use configureInjector and mockPackage     7ef665dc
* test(base/aliasMap): use configureInjector and mockPackage      e641efd3
* test(base/computePathsProcessor): use configureInjector and mockPackage     2528b445
* test(base/createDocMessage): use configureInjector and mockPackage      5d45118f
* test(base/debugDumpProcessor): use configureInjector and mockPackage      4b4eeb9e
* test(base/encodeCodeBlock): use configureInjector and mockPackage     54d6d19a
* test(base): use mockPackage     e6366e83
* test(base/templateFinder): use configureInjector and mockPackage      1b8559e3
* test(base/trimIndentation): use configureInjector and mockPackage     176d6241
* test(mockPackage): add a mock package to be used in testing     293563c3


#### link `node_modules/dgeni-package` -> `..`

To make it easier to reference modules within dgeni-packages, preinstall and postinstall
hooks are now in place to create a soft link to the root of the projet from within node_modules:

* chore(package.json): add link to this module in node_modules     68a08ec3
* chore(package.json): make node_module linking more tolerant     bfbe201b


#### writeFile Service

* feat(base/writeFile): add simple service to write a file to disk       1c9681e9
* feat(base/writeFile): add simple service to write a file to disk       f035c854
* refact(base/writeFilesProcessor): user writeFile service       aa3be581
* refact(base/debugDumpProcessor): use writeFile service     adc64c7c

### Bug Fixes

* fix(generateComponentGroup processor): ensure doc has a name     27469bec
* fix(jsdoc/codeNameProcessor): don't override codeName if already provided    942a72f6


## v0.10.0-beta.3 15th August 2014

The major change in this release was the removal of dependency on the ES6-shim and the use of ES6 `Map` for
storing maps of information. The shimmed Map was not playing nicely with Jasmine, Nunjucks and `console.log`.
Instead these mappings are now using [`StringMap`](https://github.com/olov/stringmap), which is cleaner than
using bare objects (made from `Object.create(null)`).

Thanks as always to Stéphane for his translations and removal of unused code.

* refact(*) : remove unused dependencies     5c893d85
* refact(examples/exampleMap): rename and convert to a StringMap      bdbb7c26
* fix(ngdoc/templates): fix github links      2f01d163
* fix(examples): use computePathsProcessor for example file paths     c4b02945
* fix(examples/generateExamplesProcessor): ensure correct files are in manifest     dc60336e
* fix(ngdoc/templates): ensure github links are to valid paths      7676f187
* feat(base/readFilesProcessor): add projectRelativePath to fileInfo      7931f230
* fix(examples): ensure example index files have correct path     e5e62554
* refact(jsdoc/moduleMap): use a StringMap to store the modules     0c37674a
* refact(TagColletion) use StringMap for tagsByName property      d6655cf0
* refact(jsdoc/parseTagsProcessor): use StringMap     b61e3e20
* refact(jsdoc/inlineTagProcessor): use StringMap     33f6e5fc
* refact(computePathsProcessor): use stringmap and no longer allow default template     93fc95cf
* refact(base/readFilesProcessor): use stringmap for fileReaderMap      be33702c
* fix(ngdoc/macro.html): default param values are in `doc.    e3899b67
* fix(partialNameMap): use pure object to prevent property collisions     3750c928
* refact(*): remove dependency on 'es6-shim' and `Map`      15751dfb


## v0.10.0-beta.2 7th August 2014

Bug fixes and refactoring.  The big change in this revision is the introduction of the `computePathsProcessor`.

* refact(examples): use computePathsProcessor      f85487f7
* refact(examples/parseExamplesProcessor): ditch using ES6 Map for examples      c7d2b6db
* refact(examples/generateExamplesProcessor): ditch using ES6 Map for examples       a770bf91
* refact(examples/runnableExample inlineTag): ditch using ES6 Map for examples       f1b463dc
* feat(examples/generateProtractorTestsProcessor): add new processor from Angular.js       c08b9be4
* refact(examples/examples): ditch using ES6 Map       37ac555c
* fix(ngdoc): ensure API docs go into 'partials' folder      e9aa9f81
* fix(ngdoc/generateComponentGroupsProcessor): use moduleName and moduleDoc rather than module       a0f32a03
* fix(ngdoc/module tagDef): don't calc module if docType is "overview"       ba819910
* fix(ngdoc/area tagDef): docs now use relativePath not filePath       620a2b07
* fix(createDocMessage): docs now use relativePath not filePath      efb7397c
* fix(computePaths): use log.debug not console.log       1a8f18ba
* refact(examples/templates): move files up a folder       7e7fdea5
* feat(base/createDocMessage): include docType in message       7add32a5
* feat(base/computePathsProcessor): improve error messages        14086ed2
* refact(examples): use computePathProcessor from base package        f6891e9b
* fix(computeIdProcessor): don't compute if id is already defined       bab945be
* refact(ngdoc): use computePathProcessor from base package       fe187590
* fix(jsdoc): add 'js' docType path template        a3d5f5b1
* feat(jsdoc file-reader): give each read doc a `docType` of `"js"`       2f15a7cf
* refact(jsdoc): use computePathProcessor from base package       90adbf8b
* refact(jsdoc/computePathProcessor): use the computePathProcessor from base package        a2e7a6f8
* feat(computePathsProcessor): add configurable processor       15179ce5


## v0.10.0-beta.1 25th July 2014

**This is a major rearchitecture in line with changing to
[dgeni@0.4.0](https://github.com/angular/dgeni/blob/master/CHANGELOG.md#v040-beta1-25th-july-2014)**

There are numerous breaking changes surrounding this release and that of dgeni 0.4.0.
The most important changes are

* Configuration is done directly on the Processors and Services using Configuration Blocks, which
are defined on Packages.
* Everything is now dependency injected. Dgeni deals with instantiating Processors and Services
  but if you have properties on these that reference objects that should also be instantiated by the
  DI system then you can either ask for them to be injected into the config block:

  ```js
  myPackage.config(function(processor1, someObj) {
    processor1.someProp = someObj;
  });
  ```

  use the `injector` directly:

  ```js
  myPackage.config(function(processor1, injector) {
    processor1.someProp = injector.invoke(someObjFactory);
  });
  ```

  or use the `getInjectables()` helper service:

  ```js
  myPackage.config(function(processor1, getInjectables) {
    processor1.someProp = getInjectables([someObjFactory, someOtherObjFactory]);
  });
  ```

* All real processors have changed their names from dash-case to camelCase. This is because it is
easier for their names to be valid JavaScript identifiers.

The most significant commits are:

* fix(utils/code): encode HTML entities  13b99152
* feat(base/debugDumpProcessor): add new processor   4c126792
* feat(dgeni package): add initial package for documenting dgeni configurations  2bfa92b2
* refact(parseExamplesProcessor): use Map() for example.files       d926879a
* fix(ngdoc/module tag-def): module is the first segment of the relative path       649f3051
* fix(jsdoc/description tag-def): capture non-tag specific description        ed68438d
* feat(base/createDocMessage): add new service        db11bc44
* fix(*): doc.file is now doc.fileInfo.filePath       fb600502
* fix(ngdoc/collectPartialNamesProcessor): compute-id was renamed to computeIdProcessor       0158fb3b
* fix(ngdoc/apiDocs): compute-path was renamed to computePathProcessor        9396f8c3
* fix(ngdoc/apiDocsProcessor): compute-id was renamed to computeIdProcessor       a83d7fc9
* feat(ngdoc package): add getTypeClass service       addebf63
* refact(base/code): rename to encodeCodeBlock        2ae134ff
* feat(getTypeClass): add new service       9c49ff9d
* fix(ngdocFileReader): must have an explicit name        9c5dd397
* test(nunjucks/templateEngine): templateEngine now relies on templateFinder        0269acf5
* fix(nunjucks/marked custom tag): add service name for DI injection       9069c24f
* refact(trimIndentation): convert to DI service        3ab6c9ed
* fix(nunjucks/templateEngine): get the templateFolders from the templateFinder       8760aa7f
* fix(inlineTagProcessor): inline tag definitions are optional        380dd474
* fix(computePathProcessor): let writeFileProcessor deal with outputFolder        4057deb8
* fix(jsdoc fileReader): file-readers need explicit names       cad6d043
* fix(jsdoc package): pseudo processors need to use $runBefore, etc.        5d32020f
* fix(renderDocsProcessor): extra and helpers and optional        6bc1f16a
* fix(readFilesProcessor): resolve include and exclude paths correctly        f7ea5f78
* refact(computePathProcessor): read outputFolder config from writeFilesProcessor       828b48c3
* feat(api-docs): allow packageName to be specified as a tag        83c7e1fa
* fix(jsdoc package): add trimWhitespaceTransform to package        75f52df1
* refact(templateFinder): now call getFinder() to get the actual function       e8c015d9
* refact(jsdoc transforms): convert to DI services        5e92ff46
* feat(ngdocs/moduleMap): add new service to support apiDocsProcessor et al       19a37a27
* fix(runnableExample inline-tag): examples is now a Map        d1857779
* test(tag-defs): split out tests into separate files       9be421f7
* fix(jsdoc package): jsdocFileReader should be loaded as a service       0c92271c
* refact(ngdoc/tag-defs): convert to DI injectables       d8512597
* refact(ngdoc/link inline tag): convert to DI injectable       77e51df3
* refact(ngdoc/code tag): convert to DI injectable        1d23cd4e
* refact(ngdoc/code filter): convert to DI injectable       8c871b3d
* feat(getLinkInfo): add new service        32aa8427
* refact(partialNameMap): rename and convert to DI service        49acc949
* feat(getPartialNames): add new service        c6326268
* feat(parseCodeName): add new service        e02fe91c
* refact(base/services): move code and trimIndentation to be DI services        00d17816
* refact(examples service): move to its own service (as part of no-config update)       16d7819e
* refact(renderDocsProcessor): templateEngine now has a `getRenderer()` method        4f50737b
* refact(jsdoc): convert transforms to services       6dc5417f
* refact(extractTagsProcessor): move computation into smaller functions       fa1821c1
* refact(tagExtractor): move into the extractTagsProcessor        49e51da4
* refact(tagParser): move into the parseTagsProcessor       efba4e9b
* feat(read-files): add path exclusion and update to no-config        6853d759
* refact(*): update to use new processor configuration style        c54fd8d6
* refact(*): use new dgeni Packages       128c2e61



## v0.9.3 05/22/2014

* fix(extract-type): cope with missing type   4584a423

## v0.9.2 05/09/2014

* fix(jsdoc package): trim whitespace from tags   afa5c8c6

## v0.9.1 05/02/2014

* fix(ngdoc/compute-path): use ngdoc specific version of this processor  3e17d31b
* fix(code-name): cope with additional code situations   8b456b08
* fix(jsdoc/trim-whitespace transform): only trim strings   5aa2376d
* fix(jsdoc/jsdoc file-reader): cope with comments that have no code node   4e3857db
* fix(code-name): recognise CallExpression nodes   14c5c103

## v0.9.0 05/01/2014

This is a major refactoring release which is compatible with Dgeni v0.3.x. There
are many breaking changes.

### New Packages

The packages have been refactored into smaller more focussed sets of processors.

* base - The minimal set of processors to get started with Dgeni
* jsdoc - Tag parsing and extracting
* nunjucks - The nunjucks template rendering engine. No longer in jsdoc - you must add this
  explicitly to your config or you will get
  `Error: No provider for "templateEngine"! (Resolving: templateEngine)`
* ngdoc - The angular.js specific tag-defs, processors and templates.  This loads the jsdoc and
  nunjucks packages for you.
* examples - Processors to support the runnable examples feature in the angular.js docs site.

### New Processor Exports

With Dgeni 0.3.0 processors can declaratively export services to be injected into processors'
`process()` method. This release take full advantage of this, refactoring the structure of the
dependencies of various processors to simplify and enable more flexibility.

### New Tag Definition Transforms

Previously processing of tags was somewhat distributed between the tagParser and the tagExtractor,
with various features rather hard-coded, such as `canHaveType` and `canHaveName`.  This has all been
moved into **tag definition transforms**, which provide a much more flexible and powerful way to
define how to transform the simple text "parsed" from the tag into a rich object that can be
attached to the document.

### Detailed List of Changes

**Features**

* feat(jsdoc/tag-defs): add `@type` tag       904aa00b
* feat(jsdoc/tag-defs): add `@method` tag       6fc99313
* feat(jsdoc file-reader): add more code metadata        7820317a
* feat(jsdoc/name-from-code): extract the name of the doc from the code        1115c431

**Refactorings**

* refact(ngdoc/tag-defs): use new tagExtractor syntax       b0848557
* refact(jsdoc/tag-defs): use new tagExtractor syntax       0048547e
* refact(extract-tags processor): rename and use tagExtractor       d2ef2237
* refact(tagExtractor): major reworking to use 'transformFns'       a90734ae
* refact(parse-tags): simplify using tagParser        02cc093d
* refact(tagParser): move into its own processor        1d2e689e
* refact(tagDefinitions): move into its own processor       d2d916ef
* refact(defaultTagTransforms): move into its own processor       354a9489
* refact(tag-def/transforms): convert "tagProcessors" into tag "transforms"        d4ca4e94
* refact(nunjucks): move basic filters and tags to nunjucks package        5547409c
* refact(dash-case): change name to change-case        39ab9be1
* refact(walk): remove unused code         66f86a50
* refact(marked): remove unused code         4591bd90
* refact(doc-writer): remove unused code         41c0cd12
* refact(dash-case): remove unused code        8f9dd805
* refact(check-property): remove unused code         6e39ba70
* refact(code-name): move to jsdoc package         4061e64f
* refact(packages): align with renames and moves of processors         a21f804e
* refact(doc-extractor): complete rename to read-files         8bc760bf
* refact(escaped-comments): rename to unescape-comments        d030ca95
* refact(rendering): move nunjucks stuff out         0b36e95a
* refact(code-name): rename        6e312504
* refact(doc-extractor): rename to read-files        60ac908c
* refact(partial-names processor): remove `init` and provide `exports`         0de2680a
* refact(component-groups-generate processor): remove `init` and provide `exports`         61ba9cb1
* refact(api-docs processor): remove `init` and provide `exports`        34d05b1f
* refact(jsdoc processors): remove `init` and provide `exports`        3188ff14
* refact(examples-parse): remove `init` and provide `exports`        5cbcbab6
* refact(examples-generate): remove `init` and provide `exports`         0c006bb4
* refact(nunjucks-renderer): remove `init` and provide `exports`         f4b42dd6
* refact(doc-extractor): remove `init` and provide `exports`         fce833c9
* refact(*): update due to utils move        0245eb22
* refact(utils): moved here from dgeni         1f04843d
* refact(jsdoc): moved stuff to base package         5f2ec6be

**Bug Fixes**

* fix(tagExtractor): invalid injectable parameter name        6c8790f3
* fix(jsdoc): add defaultTagTransforms and tagExtractor processors        12ac7aa0
* fix(jsdoc): tag-extractor processor was renamed       1931f4d4
* fix(tagExtractor): accidental global vars       5de56780
* fix(extract-type transform): ensure tag.description gets updated        0f911d8a
* fix(extract-name transform): ensure tag.description gets updated        e347c847
* fix(tagDefinitions): throw error if tag definitions are missing from the config       4777ec79
* fix(nunjucks): correctly load up the template engine processor         071e52c7
* fix(base processors): minor fixes to get the tests working         efd3e35f
* fix(link inline tag): parse newlines in link's title       b2ebb415
* fix(ngdoc): don't show first param in filter syntax        4f2ccf52
* fix(walk): hack ancestor to kind of do what I want         f19b6940
* fix(compute-path): ensure it runs early enough         fe1e0bd7
* fix(jsdoc package): actually append processors to config         f2020d47
* fix(marked tag): fix path to trim-indentation module         1206f8fe
* fix(nunjucks-renderer): `env` changed to `templateEngine`        e4a756e0
* fix(base package): load change-case filter locally         a74f2ee4
* fix(compute-paths): ensure it is run before rendering        b50baa99
* fix(jsdoc/tag-defs): Allow multiple `@see` tags        d73a842f
* fix(tag-parser): don't overwrite default tag processors collection         9fc7f58e
* fix(code): fix path to utilities         26c26e70
* fix(examples-parse): fix path to utilities         1f9d1488
* fix(jsdoc/tag-defs): missing comma         293ffde2
* fix(jsdoc): fix typo in error message       b1e7dd08


## v0.8.3 04/23/2014

**Bug Fixes**

* fix(ngdoc): don't show first param in filter syntax   9c5a7f26
* fix(jsdoc): fix typo in error message   b1e7dd08


## v0.8.2 03/22/2014

**Bug Fixes**

* fix(jsdoc/jsdoc-extractor): ensure Windows newlines are respected    7f1e1627
* fix(jsdoc/jsdoc-extractor): fix off-by-one error    fedcf6b1
* fix(jsdoc/lib/walk): also walk the keys of properties   4a8ae60d
* fix(jsdoc/nunjucks-renderer): improve error message   554c7afd


## v0.8.1 03/18/2014

**Bug Fixes**

* fix(examples/index.template): nunjucks uses `not` not `!`   e0070e3f


## v0.8.0 03/18/2014

**New Features**

* feat(examples/index.template): allow ng-app to be defined in the example    9b760c08
* feat(jsdoc package): use `jsdoc` rather than `js` doc-extractor   72866263


## v0.7.1 03/11/2014

**Minor Features**

* feat(api-docs): add configuration for paths  8ddcf647
* feat(runnableExample template): provide the path to the example  353eef6e


## v0.7.0 03/11/2014

**New Features**

* feat(TagCollection): add an array of Tags via the constructor 7c1cca1a
* feat(jsdoc/tag-defs): add deprecated tag  0f3a1949
* feat(examples-generate): create manifest.json file for Plunker  1849ec49

## v0.6.0 03/07/2014

**New Features**

* feat(tagParser): only ignore tags that are defined with ignore property 59492bea
* feat(jsdoc tags): improve jsdoc tag coverage  d8eb2b43
* feat(PartialNames): getLink disambiguates docs by area  6da98dd5
* feat(jsdoc/compute-paths): add new processor  23cc829a
* feat(partial-names): add removeDoc method 746a0bc7
* test(link handler): fix test, since the handler now throws on error a15053ab

**Bug Fixes**

* fix(compute-paths): ensure contentsFolder is applied correctly  301877fc
* fix(filter-ngdocs processor): run before tags are extracted a090cf49

**Refactorings**

* refact(ngdoc/id tag def): move functionality to its own doc processor 268ac3bd
* refact(partial-name processor): move adding docs to own processor 8684226b

**BREAKING CHANGE**

* If you relied on undefined tags being quietly ignored
your processing will now fail.  You should add new tag defintions for
all tags that you wish to ignore of the form:

```
{ name: 'tag-to-ignore', ignore: true }
```


## v0.5.0 03/07/2014

**New Features**

* feat(jsdoc extractor): add next code node to the doc  22a59651

**Bug Fixes**

* fix(jsdoc extractor): ignore non-jsdoc comments  50ad83d8
* fix(inline link tag): throw error if link is invalid   07af2f42

## v0.4.0 03/06/2014

**New Features**

* feat(examples): move injected example into a template  cc658f31
* feat(jsdoc): add `rendering.nunjucks.config` field to config  eb805097
* feat(link inline handler): replace old link processor with new inline handle  723e0e56
* feat(inline-tag processor): add new generic inline tag processor  39083631
* feat(firstParagraph filter): add new filter  4dcabba1
* feat(jsdoc extractor): add esprima powered jsdoc extractor  e96da1ea

**Bug Fixes**

* fix(ngdoc/templates) : improve "View Source" and "Improve Doc" links  049ee59f
* fix(write-files): ignore docs that have no output path  c666e5e3
* fix(ngdoc templates): show first paragraph not first line  7335fd91

**BREAKING CHANGE**

* The `examples` injectable object has changed from being
a flat array to a hash indexed on the id of the example.  If you only
iterated over the examples then things like `forEach` should still just
work.  But you can no longer access the examples by index, e.g.
`examples[0]` will return undefined rather than the first example.

## v0.3.1 03/02/2014

**Bug Fixes**

* fix(tagParser): don't break on bad-tags  560eff7b


## v0.3.0 02/28/2014

**New Features**

* feat(tagParser): ignore tags inside fenced code blocks   09fb7d64
* feat(trimProcessor): add tag processor to trim off whitespace  a81f6231
* feat(nameProcessor): add support for param aliases   5720bfed

**Bug Fixes**

* fix(typeProcessor): handle escaped braces  786f1ab5
* fix(ngdoc templates): ensure type hints are escaped  4ace02b8
* fix(escaped-comments): re-code HTML escaped comment markers  020fde5c
* fix(examples-parse): ensure that code blocks are rendered correctly  10ae5e21
* fix(api-docs processor): don't contaminate the global context  2fa8acf6
* fix(typeProcessor): add better error message   6becbd46
* fix(tag-parser): add better error message  458b26f5
* fix(tagParser): cope with tags that have no following whitespace   04cf4f02
* fix(typeProcessor): attach optional property to tag if type is optional  0188305f


## v0.2.4 02/25/2014

**Bug Fixes**

* fix(doctrine-tag-parser): don't rethrow error if tag type is bad  7ac46af6

## v0.2.3 02/25/2014

**Bug Fixes**

* fix(doctrine-tag-parser): support jsdoc3 tags and improve error messages  c8ca67a2

## v0.2.2  02/21/2014

**Bug Fixes**

* fix(examples-generate): ensure each index file gets content c4918e05
* fix(ngdoc/members): render member docs correctly  c7b98a67

## v0.2.1 02/20/2014

**Bug Fixes**

* fix(example-generation): commonFiles should get scripts from the 'scripts' object  3b41c91a

## v0.2.0 02/20/2014

**New Features**

* feat(example-generation): generate examples for multiple deployments  82ba9054

## v0.1.0 02/20/2014

**Bug Fixes**

* fix(doc-extractor): give decent error if projectPath is missing 0e326692
