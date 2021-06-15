# Site Development Notes

## How To Run A Local Dev Instance (OS X)

Install Ruby 2.7  
```brew install ruby@2.7```

Create an env.sh file to add the new Ruby installation to your path 
```
set DIR (cd (dirname (status -f)); and pwd) 
export PATH="/usr/local/opt/ruby@2.7/bin:$PATH"
```

Source the envelope  
```. env.sh```

Install Bundler  
```gem install bundler```

Now, whenever you want to run a local development version of the site, simply source your env.sh file, cd into your source directory, then run:  
```bundle exec jekyll serve```

