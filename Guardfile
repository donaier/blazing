guard :rspectacle, :version => 2, :cli => "--colour --fail-fast --format nested" do
  watch('spec/spec_helper.rb')                        { %w(spec/spec_helper spec) }
  watch(%r{^spec/.+_spec\.rb})
  watch(%r{^lib/(.+)\.rb})     { |m| "spec/#{m[1]}_spec.rb" }
  watch(%r{^lib/blazing/(.+)\.rb})     { |m| "spec/blazing/#{m[1]}_spec.rb" }
  watch('spec/spec_helper.rb') { "spec" }
  watch(%r{^lib/blazing/templates/(.+)}) { "spec" }
  watch('lib/blazing/runner.rb') { "spec/blazing/integration/*" }
end
