require 'fileutils'
PUBLIC_PATH = File.join("../../")
IMG_PATH = File.join PUBLIC_PATH, "images"
JS_PATH = File.join PUBLIC_PATH, "javascripts"
CSS_PATH = File.join PUBLIC_PATH, "stylesheets"

namespace :tipsy do
  
  desc 'Install source files and image files to proper locations for a rails project'
  task :install do
    
    # assuming that this dir is in public/javascripts/tipsy
    js_file = File.join("./src/javascripts/jquery.tipsy.js")
    css_file = File.join("./src/stylesheets/tipsy.css")
    image_files = Dir.glob(File.join("./src/images","*.gif"))
    
    FileUtils.cp_r js_file, JS_PATH
    FileUtils.cp_r css_file, CSS_PATH
    FileUtils.cp_r image_files, IMG_PATH
    
    puts "Files installed successfully!"
    
  end
  
end
