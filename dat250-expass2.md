#technical problems that you encountered during installation and use of Java Persistence Architecture (JPA) and how you resolved

There was no javax.persistence_*.jar in the eclipseLink zip file i downloaded. Also i had the same problem as someone else in the chat with: 
Exception in thread "main" javax.persistence.PersistenceException: No Persistence provider for EntityManager named todos
at javax.persistence.Persistence.createEntityManagerFactory(Persistence.java:84)
at javax.persistence.Persistence.createEntityManagerFactory(Persistence.java:54)
at de.vogella.jpa.simple.main.Main.main(Main.java:17)

I got to set up the basic maven project.

#links to experiment 1 and 2:

1. https://github.com/EvenSandvik/DAT250STE1/tree/master/ex2/jpa-basic

2. https://github.com/EvenSandvik/DAT250STE1/tree/master/ex2/credit-card

I was able to inspect the databases in a database workbench:
https://github.com/EvenSandvik/DAT250STE1/blob/master/ex2/DB1.png?raw=true
https://github.com/EvenSandvik/DAT250STE1/blob/master/ex2/DB2.png
