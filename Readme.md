  ___   ___   ___         ___   ___         _  _                                            _           ___ 
 | _ \ / __| / __|       |_ _| |_ _|  ___  | || |  ___   _ __    ___  __ __ __  ___   _ _  | |__       |_  )
 |  _/ \__ \ \__ \        | |   | |  |___| | __ | / _ \ | '  \  / -_) \ V  V / / _ \ | '_| | / /        / / 
 |_|   |___/ |___/  ___  |___| |___|       |_||_| \___/ |_|_|_| \___|  \_/\_/  \___/ |_|   |_\_\  ___  /___|
                   |___|                                                                         |___|      


main.cpp - example of using most of the methods and functions.


Assigning new Rooms:

Cabinet(int *room's number*)		//AccessLevel - YELLOW
LectureRoom(int *room's number*)	//AccessLevel - GREEN
ConferenceRoom(int *room's number*)	//AccessLevel - YELLOW
ClassRoom(int *room's number*)		//AccessLevel - GREEN
DirectorRoom(int *room's number*)	//AccessLevel - RED


Assigning new Users:

Director(string *Director's Name*, int *Cabinet's number*)
Admin(string *Admin's Name*)
Professor(string *Professor's Name*, int *Cabinet's number*, string *Favorite joke*)
LabEmployee(string *employee's Name*, Cabinet *Lab*)
Student(string *student's Name*, int *course*)


users.cpp methods and functions:

*User*.getName() - returns string with user's name
*User*.getAccessLevel() - returns AccessLevel with user's access level
*User*.access(Room) - returns boolean with result of trying go in user in room
*User*.addCustomAccess(Admin,Room) - function, gives user access to room, mentioning admin in log
*User*.addCustomAccess(Admin,Room) - function, cancels user access to room, mentioning admin in log
*Student*.getCourse() - returns int with student's course
*Professor**Director*.getCabinet() - returns Cabinet, which is connected to professor
*Professor*.getJoke() - returns string with professor's favorite joke
*LabEmployee*.getLab() - returns Cabinet, which is connected to employee


room.cpp methods and functions:

*Room*.getNumber() - returns int with room's number
*Room*.getAccessLevel() - returns AccessLevel for exact room
*Room*.equals(Room) - returns bool 