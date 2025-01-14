Yii Framework 2 smarty extension Change Log
===========================================

2.0.11 
----------------------------------------
- Bug #38: Change call of Smarty method setTemplateDir to addTemplateDir (alex-net)


2.0.10 under development
------------------------

- no changes in this release.


2.0.9 November 19, 2019
-----------------------

- Enh #36: Added `{js}` function allowing instantiate `yii\web\JsExpression` (leandrogehlen)


2.0.8 April 16, 2019
--------------------

- Enh #31: Respect widget events (simialbi)


2.0.7 April 25, 2018
--------------------

- Bug #23: Fixed widget registration and rendering code generation inside subtemplates (eymerich)
- Enh #25: Give a choice to use SmartyBC class (a761208)


2.0.6 March 18, 2017
--------------------

- Bug #17: Updated Composer constraints to reflect the fact that it requires Smarty 3 (samdark)


2.0.5 March 17, 2016
--------------------

- Bug #12: Fixed SmartyException thrown when using multiple `{use}` for functions and blocks in inherited templates (freezy-sk)


2.0.4 May 26, 2015
------------------

- Bug #8: Fixed `functionRegisterJsFile` position parameter (TomassunGitHub, samdark)

2.0.3 March 01, 2015
--------------------

- Bug #6845: Fixed incorrect implementation of `{registerCssFile` and `{registerJsFile` (TomassunGitHub, samdark)
- Bug #6991: Fixed exception when using `{use class='yii\bootstrap\Nav' type='function'}` (ivanlemeshev)


2.0.2 January 11, 2015
----------------------

- no changes in this release.


2.0.1 December 07, 2014
-----------------------

- Bug #5748: `{path` was generating absolute URLs instead of relative ones (samdark, motzel)


2.0.0 October 12, 2014
----------------------

- no changes in this release.


2.0.0-rc September 27, 2014
---------------------------

- Enh #4619 (samdark, hwmaier)
    - New functions:
        - `url` generates absolute URL.
        - `set` allows setting commonly used view parameters: `title`, `theme` and `layout`.
        - `meta` registers meta tag.
        - `registerJsFile` registers JavaScript file.
        - `registerCssFile` registers CSS file.
        - `use` allows importing classes to the template and optionally provides these as functions and blocks.
    - New blocks:
        - `title`.
        - `description`.
        - `registerJs`.
        - `registerCss`.
    - New modifier `void` that allows calling functions and ignoring result.
    - Moved most of Yii custom syntax into `\yii\smarty\Extension` class that could be extended via `extensionClass` property.
    - Added ability to set Smarty options via config using `options`.
    - Added `imports` property that accepts an array of classes imported into template namespace.
    - Added `widgets` property that can be used to import widgets as Smarty tags.
    - `Yii::$app->params['paramKey']` values are now accessible as Smarty config variables `{#paramKey#}`.
    - Added ability to use Yii aliases in `extends` and `require`.

2.0.0-beta April 13, 2014
-------------------------

- no changes in this release.

2.0.0-alpha, December 1, 2013
-----------------------------

- Initial release.
