# -*- coding: utf-8 -*-
require "bundler/gem_tasks"
$:.unshift("/Library/RubyMotion/lib")
require 'motion/project/template/ios'
require 'bundler'
Bundler.require(:default)

require 'motion-cocoapods'

require 'motion_model'
require 'motion_model/array'
require 'motion_model/sql'

$: << File.expand_path('/lib', __FILE__)

require 'motion_model'

Motion::Project::App.setup do |app|
  # Use `rake config' to see complete project settings.
  app.name = 'MotionModel'
  app.delegate_class = 'FakeDelegate'
  app.detect_dependencies = false

  app.pods do
    pod 'FMDB', '2.1'
  end
end
