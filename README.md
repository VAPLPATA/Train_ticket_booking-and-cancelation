# Train_ticket_booking-and-cancelation

def __init__(self,name,fare,seat):
        self.name=name
        self.fare=fare
        self.seat=seat
    
    def getStatus(self):
        print(f"The Name of the passanger is {self.name} ")
        print(f"The fare of the passanger is {self.fare} ")
        print(f"The seat number of seats availble are {self.seat} ")
        print("##########################################")


    def bookTicket(self,seat):
        n=len(seat)
        print(n)
        if n > 0:
            print(f"You can Book ticket and your seat number will be {seat.pop(n-1)}")
            
            
        else:
            print("All seats are Full please try in tatkal")

        print("##########################################")



    def cancleTicket(self,seat):
        print("Do you want ot cancel ticket")
        ans=input("Enter 'y' for Yes and 'n'for NO ")
        if ans=='y':
            seatNo=input("Enter a seat number which you want to cancel")
            seat.append(seatNo)
            print(f"Now seats available are {seat}")
        else:
            print(f"Your seat number is {len.seat()}")
        

ticket=Train("Mandavi Express: A-234", 90,['0','1','2','3','4','5','6','7','8','9'])

ticket.getStatus()
ticket.bookTicket(['0','1','2','3','4','5','6','7','8','9']) 
ticket.getStatus()
ticket.cancleTicket(['0','1','2','3','4','5','6','7','8','9'])
