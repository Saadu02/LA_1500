# LA_1500 Lern-Bericht

Joël Haldimann, Sathana Suganthasri, Kilian Stäuble

## Einleitung

Wir haben mit Unity ein Tower-Defense Spiel programmiert.

## Was haben wir gelernt?

Wir haben gelernt wie ein Item aus Unity einem vorgeschriebenen Pfad folgen können.

## Beschreibung

In userem Projekt mussten die Gegner einem Vorgeschreibenen Pfad folgen, sodass diese dann vom Punkt A oder dem Start via den Weg zum Ende kommen. Anfangs hatten wir
nur wenig bis gar keine Ahnung und wir waren auch ziemlich verwirrt von Unity, da Unity deutlich komplizierter war als erwartet. Wir waren ein wenig ratlos, denn wir 
dachten, dass es anfangs nicht so kompliziert sein würde. Wir haben dann zuerst im Unity Hub nach Tutorials gesucht, diese waren allerdings nur wenig hilfreich und wir
suchten weiter. Als wir dann ganz allgemein im Internet nach Hilfe suchten, fanden wir schnell, was wir benötigten. Es gab viele Tutorials und auch genau die, die wir
brauchten. So konnten wir richtig anfangen. Aber als wir die Map programmierten und versuchten, dass die Gegner dem Weg folgten, gab es auch schon wieder Probleme, denn
wir hatten viele Fehler in userem Code und wir wussten nicht wo diese waren, doch nach langer Fehlersuche funktionierte dies dann auch endlich.


### Code für Waypoint
``` csharp
public class Waypoints : MonoBehaviour
{
    //creates array, which can save positions
    public static Transform[] points;

    void Awake()
    {
        //the position of the waypoints in the folder get saved into the array
        points = new Transform[transform.childCount];
        for (int i = 0; i < points.Length; i++)
        {
            points[i] = transform.GetChild(i);
        }
    }

}

```

###Code für Gegner
``` csharp
void Start()
    {
        //The first waypoint gets set as target
        target = Waypoints.points[0];
    }

    void Update()
    {
        //the enemy targets the firs enemy and moves towards it
        Vector3 dir = target.position - transform.position;
        transform.Translate(dir.normalized * speed * Time.deltaTime, Space.World);

        if (Vector3.Distance(transform.position, target.position) <= 0.4f)
        {
            //When this gets trigered, the enemy has reached the waypoint
            GetNextWaypoint();
        }
    }
```
