FooTable-rails
==============

footable-rails integrates [FooTable](https://github.com/bradvin/FooTable) in Rails assets pipeline.

1. Gemfile
```
gem 'footable-rails'
```

2. Add to application.css before *= require tree
```sass
*= require footable-rails
```

3. Add to application.js before //= require tree
```
//= require footable-rails
```

4. Initialize FooTable!

There should be a match between <table class="my_footable"> and ".my_footable"
```html
<script type="text/javascript">
    $(function () {
        $('.my_footable').footable();
    });
</script>
```