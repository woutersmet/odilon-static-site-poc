source "https://rubygems.org"

# Match the Jekyll version GitHub Pages runs. Locally on Ruby 2.6 the
# constraints below pull older compatible dependencies; on the Actions
# runner (Ruby 3.2) newer compatible versions resolve automatically.
gem "jekyll", "~> 3.10"

# Constraints needed only on legacy Ruby (2.6). Harmless on newer Rubies.
install_if -> { RUBY_VERSION < "3.0" } do
  gem "ffi", "< 1.17"
  gem "public_suffix", "< 5.0"
  gem "google-protobuf", "< 3.22"
  gem "rexml", "< 3.3"
end

gem "webrick", "~> 1.8" # needed for `jekyll serve` on Ruby 3+
