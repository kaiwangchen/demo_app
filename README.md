http://ruby.railstutorial.org/chapters/a-demo-app

    rails new demo_app --skip-bundle

    cd demo_app
    subl Gemfile
    bundle install --without production

    subl .gitignore

    mv README.rdoc README.md
    subl README.md

    git init
    git add .
    git commit -m "Initial commit"

    git remote add origin git@github.com/kaiwangchen/demo_app.git
    git push -u origin master

    rails generate scaffold User name:string email:string
    bundle exec rake db:migrate

    rails server  # http://localhost:3000/users

    rails generate scaffold Micropost content:string user_id:integer
    bundle exec rake db:migrate

    rails server  # http://localhost:3000/microposts

    # http://ruby.railstutorial.org/chapters/a-demo-app#sec-mvc_in_action
    # rails console

    rake assets:precompile
