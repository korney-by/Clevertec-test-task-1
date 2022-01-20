import javafx.geometry.Point3D
import kotlin.math.pow
import kotlin.math.sqrt

fun main() {
    val messageTextDistance = "Distance between Point %d and Point %d: %s"
    val messageTextFullDistance = "All distance: %s"

    val points = arrayOf(
        Point3D(2.0, 1.0, 3.0),
        Point3D(7.0, 5.0, 8.0),
        Point3D(4.0, 2.0, 3.0)
    )
    var fullDistance = 0.toDouble()
    for (i in 0 until points.size - 1) {
        val distance = points[i].distanceTo(points[i + 1])
        println(String.format(messageTextDistance, i + 1, i + 2, distance))
        fullDistance+=distance
    }
    println(String.format(messageTextFullDistance, fullDistance))
}

fun Point3D.distanceTo(point: Point3D): Double {
    return sqrt((this.x - point.x).pow(2.0) + (this.y - point.y).pow(2.0) + (this.z - point.z).pow(2.0))
}
