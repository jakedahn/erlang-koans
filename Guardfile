# sudo gem install guard-shell --no-ri --no-rdoc

guard :shell do
  watch(/^Makefile|.*\.(erl|escript)$/) do |m|
    title = 'Koans'
    eager 'escript koans'
    status = ($?.success? && :success) || :failed
    n '', title, status
    ''
  end
end
