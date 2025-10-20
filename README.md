function toPercentage(value: number, total: number): number {
  return (value / total) * 100;
}

function fromPercentage(percentage: number, total: number): number {
  return (percentage / 100) * total;
}

export { toPercentage, fromPercentage };
<!doctype html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Percentage</title>
  </head>

  <body>
    The percentage of 10 out of 100 is <span id="percentage"></span>
    <script type="module">
      import { toPercentage } from "./src/main";
      document.getElementById("percentage").innerText = toPercentage(10, 100);
    </script>
  </body>
</html>
