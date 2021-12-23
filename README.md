# Timeline.js

The "HTML"
       

         <html>
           <body>
              <div id="timeline"><div>
             <script src="path/to/timeline.js"></script>
           <body>
         <html>
       

     
Define your data
       


         const timelineData = [
              {
                  'time': 'Jan',
                  'events': [
                      'A nice month to start a year',
                      'Roses are red',
                  ],
              },
              {
                  'time': 'Feb',
                  'events': [
                      'Violets are blue',
                      'No. They are kind of purple',
                  ],
              },
              {
                  'time': 'Mar',
                  'events': [
                      'Lorem ipsum',
                      'That is how it works',
                  ],
              },
              {
                  'time': 'Apr',
                  'events': [
                      'Twinkle, twinkle, little star',
                      'Rain rain go away',
                  ],
              },
         ];
       

     
Configure your timeline
       


      const timelineConfig = {
              'lineColor': '#0099ff',
              'dotColor': '#1C2333',
              'eventBackground': '#2B3245',
              'eventText': '#acc'
      };
       

     
Initialize the timeline
       


      let timeline = new TimeLine(
            'timeline', //id selector
            timelineConfig, //pass empty object if you want to use default styling
            timelineData //timeline data
      );
       

     
Draw the timeline
       

      timeline.draw();
       
