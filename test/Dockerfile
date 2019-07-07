FROM jetty
RUN rm -rf /var/lib/jetty/webapps/ROOT.war
COPY companyNews.war /var/lib/jetty/webapps/ROOT.war
RUN rm -rf $JETTY_HOME//webapps/ROOT.war
COPY companyNews.war $JETTY_HOME/webapps/ROOT.war
RUN java -jar "$JETTY_HOME/start.jar" --create-startd --add-to-start=jmx,stats
