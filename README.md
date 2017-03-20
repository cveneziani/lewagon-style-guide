# Style Guide for Le Wagon student projects

## How to install it

Edit your `config/routes.rb` file and add at the end of the routes:

```ruby
  # static pages
  get 'styleguide', to: 'pages#styleguide'
```

Edit the controller and add `styleguide` action:

```ruby
# app/controllers/pages_controller.rb
def styleguide
  @base_font   = "Open Sans"
  @header_font = "Raleway"
end
```

Edit `app/assets/pages/_index.scss` and add the following line:

```
@import "styleguide";
```

Download `_styleguide.scss` and put it inside `app/assets/stylesheets/pages/` folder.

Download `styleguide.html.erb` and put it inside `app/views/pages/` folder.

## How to add a color

1. Add a new color inside `app/assets/styleheets/config/_variables.scss`
2. Edit `app/views/pages/styleguide.html.erb` and insert your new color in the `Colors` section.
3. Edit `app/assets/stylesheets/pages/_styleguide.css` to add a new CSS class for your color.

## How to add a component

1. Create a new file for your component inside `app/assets/stylesheets/components/` folder.
2. Add CSS rules for your component.
2. Edit `app/views/pages/styleguide.html.erb` and inset the HTML code for your component.
