# Java_EE_Udemy28
Adding new JPA entity classes for flight and airplane

Creating new JPA entity classes for flight and airplane. Created Enum called FlightDestinations with names of destinations stored in String form
Created id using 
      @Id
      @GeneratedValue(stategy=GeneratedType.AUTO)
      private Integer id;
This enables the database to create the id automatically

      @Enumerated(EnumType.STRING) //calls up the Enum for FlighDestinations and declares return type
	    private FlightDestinations flightOrigin;
	
	    @Enumerated(EnumType.STRING)//calls up the Enum for FlighDestinations and declares return type
	    private FlightDestinations flightDestination;
	
	    private Integer price;
	
	    @Temporal(TemporalType.TIMESTAMP)//declares the use of TIMESTAMP for Date which includes date and time
	    private Date flightTime;
      
      
