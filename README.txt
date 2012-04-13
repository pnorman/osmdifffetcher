Instructions for use in your project (assuming you're using git)

git submodule add git://github.com/pnorman/osmdifffetcher.git osmdifffetcher

then from your python file

include osmdifffetcher

myfetcher = osmdifffetcher.DiffFetcher()

myfetcher.init_latest()

then myfetcher.next() to get the latest diff or return none if there isn't one ready yet.