desc 'build style.json from HOCON descriptions'
task :style do
  sh 'parse-hocon hocon/style.conf > docs/style.json'
  sh 'gl-style-validate docs/style.json'
end

desc 'host the site for testing'
task :host do
  sh 'budo -d docs'
end

