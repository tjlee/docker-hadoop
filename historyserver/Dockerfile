FROM bde2020/hadoop-base:1.0.0
MAINTAINER Ivan Ermilov <ivan.s.ermilov@gmail.com>

ENV YARN_CONF_yarn_timeline___service_leveldb___timeline___store_path=/hadoop/yarn/timeline
RUN mkdir -p /hadoop/yarn/timeline
VOLUME /hadoop/yarn/timeline

ADD run.sh /run.sh
RUN chmod a+x /run.sh

CMD ["/run.sh"]
