from jenkins:2.60.3-alpine

# install plugins specified in https://github.com/kohsuke/jenkins/blob/master/core/src/main/resources/jenkins/install/platform-plugins.json

# install Organisation and Administration plugins
RUN /usr/local/bin/install-plugins.sh cloudbees-folder
RUN /usr/local/bin/install-plugins.sh antisamy-markup-formatter

# install Build Features plugins
RUN /usr/local/bin/install-plugins.sh build-timeout
RUN /usr/local/bin/install-plugins.sh credentials-binding
RUN /usr/local/bin/install-plugins.sh timestamper
RUN /usr/local/bin/install-plugins.sh ws-cleanup

# install Build Tools plugins
RUN /usr/local/bin/install-plugins.sh ant
RUN /usr/local/bin/install-plugins.sh gradle

# install Pipelines and Continuous Delivery plugins
RUN /usr/local/bin/install-plugins.sh workflow-aggregator:2.0
RUN /usr/local/bin/install-plugins.sh github-organization-folder:1.6
RUN /usr/local/bin/install-plugins.sh pipeline-stage-view:2.0

# install Source Code Management plugins
RUN /usr/local/bin/install-plugins.sh git
RUN /usr/local/bin/install-plugins.sh subversion

# install Distributed Builds plugins
RUN /usr/local/bin/install-plugins.sh ssh-slaves

# install User Management and Security plugins
RUN /usr/local/bin/install-plugins.sh matrix-auth
RUN /usr/local/bin/install-plugins.sh pam-auth
RUN /usr/local/bin/install-plugins.sh ldap

# install Notifications and Publishing plugins
RUN /usr/local/bin/install-plugins.sh email-ext
RUN /usr/local/bin/install-plugins.sh mailer
