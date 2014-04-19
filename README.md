###Introduction

This gem allows you to write plan HTML views for your Mithril-based applications, making it easier to collaborate with designers and other developers not familiar with the Mithril view syntax. It is based on the work that Jonathan Buchanan did on MSX and the react-rails gem.

It allows you to create views with a `.js.msx` extension.


Example: (app/assets/todo.js.msx)
```
/** @jsx m */

todo.view = function(ctrl) {
    return <div class="dude">
        <input onchange={m.withAttr("value", ctrl.description)} type="text" class="blue" />
        <small class="pea">This is small text</small>
    </div>
};
```

Be sure to include the `/** @jsx m **/` comment in your views.

###Installation

Add `gem "mithril-rails"` to your Gemfile.

###Development

This is the first release, more functionality to come, such as generating a scaffold for controllers and views for Mithril-based applications.
