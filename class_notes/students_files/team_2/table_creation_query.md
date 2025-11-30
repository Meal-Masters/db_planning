CREATE TABLE Phone_Reservations(
	Reservation_Number INT PRIMARY KEY,
	Date DATE,
	Time TIME,
	Amount_of_people INT NOT NULL,
	Availibility_Of_Table INT NOT NULL DEFAULT 1 CHECK( Availibility_Of_Table IN(1,0)),
	Name_of_Customer TEXT NOT NULL,
	Phone TEXT NOT NULL
	
)
;