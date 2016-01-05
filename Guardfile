notification :off

guard :haskell, cabal_target: 'test' do
  watch(%r{test/.+\.l?hs$})
  watch(%r{.+\.l?hs$})
  watch(%r{\.cabal$})
  callback(:start_begin) { `cabal configure --enable-tests` }
end
