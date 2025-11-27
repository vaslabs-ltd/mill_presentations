# Makefile for LaTeX document compilation on Fedora
# Usage: make fedora

.PHONY: fedora clean pdf help

# Install all necessary TeXLive packages for Fedora
fedora:
	@echo "Installing TeXLive packages for Fedora..."
	sudo dnf install -y \
		texlive-scheme-basic \
		texlive-latex \
		texlive-latex-bin \
		texlive-babel-english \
		texlive-hyphen-english \
		texlive-grfext \
		texlive-inconsolata \
		texlive-beamer \
		texlive-xcolor \
		texlive-pgf \
		texlive-amsmath \
		texlive-amsfonts \
		texlive-geometry \
		texlive-hyperref \
		texlive-lm \
		texlive-cm \
		texlive-etoolbox \
		texlive-kvoptions \
		texlive-kvsetkeys \
		texlive-ltxcmds \
		texlive-infwarerr \
		texlive-pdftexcmds \
		texlive-epstopdf-pkg \
		texlive-grffile \
		texlive-caption \
		texlive-booktabs \
		texlive-multirow \
		texlive-url \
		texlive-cite \
		texlive-natbib \
		texlive-fancyhdr \
		texlive-setspace \
		texlive-enumitem \
		texlive-listings \
		texlive-upquote \
		texlive-l3kernel \
		texlive-l3packages \
		texlive-translator \
		texlive-pgfplots \
		texlive-qrcode
	@echo "TeXLive packages installation complete!"

# Compile the PDF
pdf:
	@echo "Compiling LaTeX document..."
	pdflatex presentation.tex
	pdflatex presentation.tex
	@echo "PDF compilation complete!"

# Clean auxiliary files
clean:
	@echo "Cleaning auxiliary files..."
	rm -f *.aux *.log *.nav *.out *.snm *.toc *.bbl *.blg *.fdb_latexmk *.fls *.synctex.gz
	@echo "Clean complete!"

# Show help
help:
	@echo "Available targets:"
	@echo "  fedora  - Install all necessary TeXLive packages for Fedora"
	@echo "  pdf     - Compile the LaTeX document to PDF"
	@echo "  clean   - Remove auxiliary files"
	@echo "  help    - Show this help message"