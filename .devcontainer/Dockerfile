FROM qmcgaw/latexdevcontainer
# Docs: https://github.com/qdm12/latexdevcontainer/tree/master

# Mark as non-interactively to avoid license prompts
ENV DEBIAN_FRONTEND=noninteractive

# Install the Microsoft fonts
RUN apt update && \
    apt install -y software-properties-common && \
    apt-add-repository contrib -y && \
    apt-add-repository non-free -y && \
    apt update && \
    apt install -y ttf-mscorefonts-installer fontconfig && \
    rm -rf /var/lib/apt/lists/*

# Install the LaTeX packages
RUN tlmgr update --self && \
    tlmgr update --all && \
    tlmgr install biber babel-german xstring etoolbox hyph-utf8 setspace lipsum titlesec acronym fontspec changepage listings csquotes dehyph-exptl bigfoot biblatex biblatex-apa

# Rebuild the LaTeX format files
RUN fmtutil-sys --all
