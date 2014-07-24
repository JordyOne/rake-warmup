desc "default task"
task :default => :greet

desc "Print a nice greeting"
task :greet do
  puts "What is your name?"
  name = STDIN.gets.chomp
  puts "Hello #{name}."
end

desc "Print the current time"
task :time do
  puts Time.now
end

desc "Print your favotite food with ENV_VAR"
task :print_favorite_food do
  ENV["FAVORITE_FOOD"]= "lasagna"
  puts "Your favorite food is #{ENV["FAVORITE_FOOD"]}"
end

desc "wake up"
task :wake_up do
  puts "wake up"
end

desc "prints Get Up"
task :get_up => :wake_up do
  puts "get up"
end

desc "eat breakfast"
task :eat_breakfast => :wake_up do
  puts "eat breakfast"
end

desc "brush teeth"
task :brush_teeth => :eat_breakfast do
  puts "brush teeth"
end

desc "ready for class"
task :ready_for_class => :brush_teeth do
  puts "ready for class"
end