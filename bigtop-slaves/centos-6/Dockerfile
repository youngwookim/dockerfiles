FROM bigtop/slaves:trunk-centos-6

RUN yum install -y epel-release
RUN yum install -y R R-devel libcurl-devel openssl-devel

RUN R -e "install.packages('devtools', repos = 'http://cran.us.r-project.org')"
RUN R -e "install.packages('rmarkdown', repos = 'http://cran.us.r-project.org')"
RUN R -e "install.packages('knitr', repos = 'http://cran.us.r-project.org')"
RUN R -e "install.packages('roxygen2', repos = 'http://cran.us.r-project.org')"
RUN R -e "install.packages('testthat', repos = 'http://cran.us.r-project.org')"

RUN yum clean all
