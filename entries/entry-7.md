## Entry 7:

### Progress throughout week:
So I have my d3 skeleton my outline of it and json and now it's time to fuse them together.

 <p align = "center">
  <img src = "giphydb.gif" width="700" height="200">
</p>

<div align="left">
  JSON^
</div>   
<div align="right">
  D3^
</div>    

I have the skeleton ready and the data ready, so all that's left is to connect the data with d3 and making it interactive.
And I was searching on google how to connect d3.js with json since d3.js has different format then jQuery or javascript and checked the data nested projects to help me remember it and see a similar format.
```
const svg = d3.select("body")
                  .append("svg")
                  .attr("width", w)
                  .attr("height", h);
    
    svg.selectAll("rect")
      .data(dataset)
      .enter()
      .append("rect")
      .attr("x", (d, i) => i * 30)
      .attr("y", (d, i) => h - 3 * d)
      .attr("width", 25)
      .attr("height", (d, i) => 3 * d)

.attr("fill", function(d) {
    return "rgb(0,"+ (d * 10) + ", " + (d * 2) + ")";
});
```
^d3 outline of my project, more to be added
### Plan for this week:
Have my mvp and fix any bugs or improve in anything that has to be improved. Make my graph more interactive. 

### Takeaways:
Use google and old sep projects to help you understand a topic or help you remember how to use it. It helped me learn more of how could implement json with d3. So always use google or old sep projects to narrow down your understanding of anything your learning


 [D3 and JSON](https://www.tutorialsteacher.com/d3js/loading-data-from-file-in-d3js)
 
 [D3 and JSON other link](http://learnjsdata.com/read_data.html)