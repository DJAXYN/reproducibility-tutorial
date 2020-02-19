# reproducibility-tutorial
This is the FOSS 2020 workshop
    1  pwd
## Clone the github repo
    2  git clone https://github.com/DJAXYN/reproducibility-tutorial.git
    3  wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
    4  bash Miniconda3-latest-Linux-x86_64.sh -b -p /opt/conda
## symbolic links from conda to /bin
    5  ln -s /opt/conda/pkgs/*/bin/* /bin
    6  ln -s /opt/conda/pkgs/*/lib/* /usr/lib
    7  /opt/conda/bin/conda install -c conda-forge -y jupyterlab=1.2.3
    8  /opt/conda/bin/conda install -c conda-forge -y nodejs=10.13.0
    9  /opt/conda/bin/pip install bash_kernel
   10  /opt/conda/bin/pip install ipykernel
   11  /opt/conda/bin/python3 -m bash_kernel.install
   12  /opt/conda/bin/conda search htseq
   13  conda search htseq
   14  /opt/conda/bin/jupyter lab --no-browser --allow-root --ip=0.0.0.0 --NotebookApp.token='' --NotebookApp.password='' --notebook-dir='/scratch/reproducibility-tutorial/'
   15  /opt/conda/bin/conda search -c bioconda snakemake
   16  /opt/conda/bin/conda install -c bioconda -c conda-forge -y snakemake=5.8.1
   17  ln -s /opt/conda/bin/* /bin
   18  ln -s /opt/conda/lib/* /usr/lib
   19  ln -s /opt/conda/lib/* /usr/lib
   20  snakemake --version
   21  sudo apt-get update
   22  sudo apt-get install -y apt-transport-https ca-certificates curl gnupg-agent software-properties-common
   23  curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
   24  sudo add-apt-repository  "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
 $(lsb_release -cs) \
 stable"
   25  sudo apt-get update
   26  sudo apt-get install -y docker-ce docker-ce-cli containerd.io
   27  docker run hello-world
   28  cd /scratch/reproducibility-tutorial/
   29  ls
   30  history >> README.md
