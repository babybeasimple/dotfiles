APPS = %w(
  auth
  casebook
  consumer
  folio
  rolodex
)

class Default < Thor
  APPS.each do |app|
    desc "#{app}", "run rails command in #{app}"
    define_method "#{app}" do |*args|
      system("cd #{app} && rails #{args.join(' ')}")
    end
  end
end
