FROM ubuntu

RUN apt-get update
RUN apt-get install make -y
RUN apt-get install gcc -y
RUN apt-get install libncurses5-dev -y
COPY ./minishell /minishell
WORKDIR /minishell
RUN make

# docker run -it simian114/minishell ./minishell
