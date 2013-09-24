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
