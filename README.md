Conveyer Belt Capacity Check 

#Har brugt Console.writeline som vist i undervisning til at få programmet til at forespørge om antallet af motorer (prompt the user for the numbers of motors), herefter indtastes input. 
#int.Parse konverterer tekst (string) fra Readline til heltal (int), hvilket betyder motors = heltal (int).
#var er implicit, finder selv type variabel.

Console.WriteLine("How many motors are carrying the packages?");
var motors = int.Parse(Console.ReadLine());

#Jeg bruger Console.writeline igen til at igen indstille maskinen på spørgsmålet der skal forespørges (prompt the user for the weight of packages) og herefter indtastes input til vægt.
#Igen bruges Readline til at læse input som tekst, og konverterer til double, fordi vi ved at vægt kan være kommatal (også for at bruge nogle af de forskellige datainput fra undervisning).
#var er implicit, finder selv type variabel.

Console.WriteLine("How many kg of packages do we expect?");
var weight = double.Parse(Console.ReadLine());

#Bruger den simple var quotient (math expression) til at dividere vægten med antal motorer.
#Fordi vægten er "double" (kommatal), bliver resultatet også double (kommatal), også fordi vi ved fra opgaven at vores quotient er >=5.6.
#Vi bruger vores if funktion til vores betingelse, som er at hvis vægt/antal motorer er mindre end eller lig med 5.6 kg, så kan systemet bære vægten, hvis det er større end 5.6, kan det ikke. 

var quotient = weight / motors;
if (quotient <=5.6)

#Nu er det igen at vi bruger Console.Writeline til at få konsollen til at printe at "Yes! The conveyor belt can carry the packages.", hvis betingelsen opfyldes. 
#Og hvis betingelsen ikke opfyldes printes anden sætning: "No. The conveyor belt cannot carry the packages." Vi bruger else funktion fordi at første betingelse køres igennem og hvis ikke betingelsen opfyldes køres næste betingelse. 

{ Console.WriteLine("Yes! The conveyor belt can carry the packages."); }
else
{ Console.WriteLine("No. The conveyor belt cannot carry the packages."); }
//
