<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE hibernate-configuration PUBLIC
        "-//Hibernate/Hibernate Configuration DTD 3.0//EN"
        "http://hibernate.org/dtd/hibernate-configuration-3.0.dtd">
<hibernate-configuration>
    <session-factory>
       <property name="hibernate.connection.driver_class"> com.mysql.cj.jdbc.Driver </property>
		<property name="hibernate.connection.url"> jdbc:mysql://localhost:3306/HQL </property>
		<property name="hibernate.connection.username"> root </property>
		<property name="hibernate.connection.password"> Root </property>
		<property name="hibernate.dialect"> org.hibernate.dialect.MySQL8Dialect </property>
		<property name="show_sql">true</property>
		<!-- <property name="hbm2ddl.auto">create</property> -->
		<property name="hbm2ddl.auto">update</property>
		
        <mapping resource="Hbm.xml" />
    </session-factory>
</hibernate-configuration>
