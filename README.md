# Minero-API-Usage
Minero API - Based on coinhive-api class 

[Minero-api.php Class](https://gist.github.com/JanrikV/816d4456a93fa7ffe371fa66099d8175)

## Example

```
$api_key = new MineroAPI('YOUR_API_KEY');

// Make a simple GET request without additional parameters
$stats = $api_key->get('/stats/site');

$hashedPerSecond = $stats->hashesPerSecond;
$hashedPerSecondTitle = number_format($hashedPerSecond, 0, '.',  '.');
$hashesTotal = $stats->hashesTotal;


// Anything less than a million
$hashTotal = number_format($hashesTotal);

$xmr = $stats->xmrPending;
```
