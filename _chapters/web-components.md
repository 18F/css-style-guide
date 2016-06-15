---
title: Web Components
---

The term [web components](http://webcomponents.org/) generally refers to
dynamic components or objects that can be dropped into and composed with
HTML, but are driven primarily by JavaScript. Web components embrace a
_modular_ architecture and offer _encapsuation_ at both the JavaScript and
CSS levels of the web stack.

Here are some links to start you off:

* [WebComponents.org] is apparently a collaboration between Google and
  Mozilla, but mostly features [articles](http://webcomponents.org/articles/)
  about Google's [Polymer] framework along with links to lots of other more
  general resources
* [An Introduction to Custom Elements](http://www.smashingmagazine.com/2014/03/04/introduction-to-custom-elements/)
  on Smashing Magazine
* [Web Components Aren't Ready for Production Yet](http://developer.telerik.com/featured/web-components-arent-ready-production-yet/)
  and [the follow-up](http://developer.telerik.com/featured/web-components-ready-production/)
  about [custom elements](#custom-elements) specifically (spoiler alert:
  they are!)
* [component.kitchen] shows off some open-source web components, and provides
  a good overview of what's possible right now using various
  [frameworks](#web-component-frameworks) and
  [polyfills](#web-component-polyfills).

## Technologies
There are a number of different technologies that support web components, all
of which are in different stages of [W3C
standardization](https://www.w3.org/standards/techs/components) and browser
implementation. As of this writing (June, 2016), the most notable are:

Technology | Status | Native implementation | Polyfill(s)
:--------- | :----- | :-------------------- | :----------
[HTML templates](#html-templates) | [accepted](https://www.w3.org/TR/html5/scripting-1.html#the-template-element) | [All modern browsers](http://caniuse.com/#feat=template), except IE (supported by Edge 13+) | [webcomponentsjs](https://github.com/webcomponents/webcomponentsjs#browser-support)
[Custom elements](#custom-elements) | [draft](https://www.w3.org/TR/custom-elements/) | [Chrome only](http://caniuse.com/#feat=custom-elements); in development for Firefox and Safari; under consideration for Edge | ["v1" spec][custom elements v1]: [webcomponentsjs](http://webcomponents.org/polyfills/custom-elements/), [document-register-element]<br>["v2" spec][custom elements v2]: **none yet**
[HTML imports](#html-imports) | [draft](https://www.w3.org/TR/html-imports/) | [Chrome only](http://caniuse.com/#feat=imports); under consideration for Edge; not planned for Firefox or Safari | [webcomponentsjs](http://webcomponents.org/polyfills/html-imports/)
[Shadow DOM](#shadow-dom) | [draft](https://www.w3.org/TR/shadow-dom/) | [Chrome only](http://caniuse.com/#feat=shadowdom); under consideration for Edge; not planned for Firefox or Safari | [webcomponentsjs](http://webcomponents.org/polyfills/shadow-dom/)


[HTML imports]: http://webcomponents.org/articles/introduction-to-html-imports/
[Polymer]: https://www.polymer-project.org/
[The State of Web Components]: https://hacks.mozilla.org/2015/06/the-state-of-web-components/
[WebComponents.org]: http://webcomponents.org/
[component.kitchen]: http://component.kitchen/
[custom elements v1]: https://www.w3.org/TR/2016/WD-custom-elements-20160226/
[custom elements v2]: https://www.w3.org/TR/custom-elements/
[shadow DOM]: http://www.html5rocks.com/en/tutorials/webcomponents/shadowdom/
[template tag]: http://www.html5rocks.com/en/tutorials/webcomponents/template/
[x-tag]: http://x-tags.org/
