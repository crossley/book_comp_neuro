# Define the default make target
all: book

# Target to compile the Bookdown book
book:
	Rscript -e "bookdown::render_book('index.Rmd', 'bookdown::gitbook')"

# Target to clean up intermediate files
clean:
	rm -rf ../*.html ../style.css reference-keys.txt search_index.json
	rm bookdown_files.Rmd
	rm -rf _bookdown_files

.PHONY: all book clean

