
AM_CPPFLAGS= -fPIC -fpermissive \
-I${BOOST_HOME} \
-I${BOOST_HOME}/boost/serialization \
-I${THERON_HOME}/Include \
-I${HADOOP_HOME}/src/c++/libhdfs\
-I${JAVA_HOME}/include\
-I${JAVA_HOME}/include/linux

AM_LDFLAGS=-lc -lm -lrt -lboost_serialization -lpthread -lxs

LDADD = 	../libexecutor.a \
		${HADOOP_HOME}/c++/Linux-amd64-64/lib/libhdfs.a\
		${JAVA_HOME}/jre/lib/amd64/server/libjvm.so\
		${BOOST_HOME}/stage/lib/libboost_serialization.a \
		${BOOST_HOME}/stage/lib/libboost_serialization.so \
		${THERON_HOME}/Lib/libtherond.a

noinst_LIBRARIES=libtest.a
libtest_a_SOURCES =	Executor.cpp 
