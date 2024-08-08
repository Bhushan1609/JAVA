# Map Compute Example in Java

This example demonstrates how to use the `Map.compute` method in Java to update the value associated with a key in a `HashMap`.

## Example Code

```java
import java.util.HashMap;
import java.util.Map;

public class MapComputeExample {
    public static void main(String[] args) {
        // Create a HashMap to map numbers to their string representations
        Map<Integer, String> numberMap = new HashMap<>();

        // Add some initial values to the map
        numberMap.put(1, "One");
        numberMap.put(2, "Two");

        // Use Map.compute to update the value for key 3, or insert it if it doesn't exist
        numberMap.compute(3, (key, value) -> (value == null) ? "Three" : value);

        // Use Map.compute to update the value for key 2, which already exists
        numberMap.compute(2, (key, value) -> value + " Updated");

        // Print the updated map
        numberMap.forEach((key, value) -> System.out.println(key + " -> " + value));
    }
}
