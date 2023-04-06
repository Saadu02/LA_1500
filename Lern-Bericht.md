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

### Code für Gegner
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

https://user-images.githubusercontent.com/111045600/230307677-7f5864e2-0f59-4dad-9fdd-e5bccde8bf0a.mp4

## Verfikation

In dem ersten Code sieht man wie die Positionen der Waypoints in einem Array gespeichert werden, das haben wir so gemacht, weil man sonst alle Waypoint individuell speichern müssste und es schnell zu lags kommen könnte.

Im zweiten Code werden dann diese Positionen verwendet um die Gegner von Punkt zu Punkt zu bewegen, zuerst wird die erste Position abgerufen, dann wenn sich der Gegner bei dieser befindet, wird die Zweite abgerufen und so weiter. Die Geschwindigkeit muss mit der echten Zeit gerechnet werden, denn sonst wäre der Gegner bei vielen Frames schneller als bei Wenigen. 

Im Video sieht man dann wie sich die Gegner (violette Kugeln) von Waypoint zu Waypoint bewegen (Waypoints türkis markiert) 


# Reflektion zum Arbeitsprozess

Die Aufgabenteilung war gut und jeder wusste, was sie machen mussten. 


Als wir Online-Unterricht hatten, konnten wir unsere Projekt nicht zusammen fügen und hatten Mühe die Probleme herauszufinden. 

**VBV**: Nächste Mal, wenn es im Gruppenarbeit eine Zusammenfügen eines Projekt geht, werden wir alle an einem Ort treffen und den Projekt zusammenfügen. 



