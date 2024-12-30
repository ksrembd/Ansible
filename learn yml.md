# Learn yml
it can be stored in 2 different formats .yml or .yaml

key/ariable can be defind with a  " : "
    ex: 
        Name: "Vijay" # considered as string in " "
        age: 30   # considered as integer
        gender: "male" # considered as string in " "

    List:
        hobbies:
            - cricket
            - hockey
            - movie
    OR
        hobbies: ["cricket", "hokey", "Movie"]
        friends:
            - name: "Manoj"
               age: 31
    OR
        friends:
        -{name: "sainath",age:30}

how to change the variable/key data type
    age: !float 30  # considerd as float 30.0
    age: !str 30    # considerd as string "30.0"
    age: !str 30

long string
    desc: asldkfo8tnlkslksdfjikjlskdjflksdionslkdflksehoriahndflknsdfasekfnosindflkdfnaoseifnlskdgladfnsndfglgkadnflknsdlfknsdlfn
how to manage in differed formats 
option 1
     desc: >asldkfo8tnlkslksdfjikjlskdjflksdionslkdflks
     ehoriahndflknsdfasekfnosindflkdfnaoseifnlskdgladfn
     sndfglgkadnflknsdlfknsdlfn

option 2
    desc: | asldkfo8tnlkslksdfjikjlskdjflksdionslkdflksehoriahn
    dflknsdfasekfnosindflkdfnaoseifnlskdgladfnsndfglgkadnflkn
    sdlfknsdlfn