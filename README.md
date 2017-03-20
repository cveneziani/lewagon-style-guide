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

Download [_styleguide.scss](https://raw.githubusercontent.com/cveneziani/lewagon-style-guide/master/_styleguide.scss) and put it inside `app/assets/stylesheets/pages/` folder.

Download [styleguide.html.erb](https://raw.githubusercontent.com/cveneziani/lewagon-style-guide/master/styleguide.html.erb) and put it inside `app/views/pages/` folder.
