
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#about-the-project">About The Project</a></li>
    <li>
      <a href="#hardware introduction">hardware introduction</a>
      <ul>
        <li><a href="#hardware used">hardware used</a></li>
        <li><a href="#hardware wiring">hardware wiring</a></li>
      </ul>
    </li>
    <li><a href="#how it works">how it works</a></li>
    <li><a href="#assessment methodology">assessment methodology</a></li>
    <li><a href="#data visualization example">data visualization example</a></li>
    <li><a href="#contact">contact</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#references">references</a></li>
  </ol>
</details>


# about-the-project
A implementation of project to use Raspberry Pi based device to detecting and evaluating sleep quality, use C++ mostly.
# how it works
We use several kinds of sensors to monitor users sleep and collect their data related to the sleep. The device, then, evaluate users' sleep quality and diagnose if users suffering from sleep disorders, according to the assessment that given below. Additionally, the diagonsis will be uploaded to a serve eventually and users are allowed to check it out by downloading it through a computer or cellphone. During the sleep, sleep infomation will also be uploaded to the serve in real time，which allows supervisors (maybe baby-sitters, parents, nurses etc.) to record users' real-time sleep state.

Here is a working demonstration of the system:
![15E17EC1-5B44-4358-8A54-BAEF73FF8F33](https://user-images.githubusercontent.com/77977624/109402512-73ac1700-794e-11eb-8671-5e314399f869.jpeg)
# assessment methodology
According to polysomnography (PSG), we are able to do a sleep study by monitoring or recording bio-physiological changes that occur in the human body when the person is asleep. Based on data collected during sleep, like brain activity, eye movements, muscle activity and heart rhythm, doctors are allowed to diagnose whether patients are suffering from sleep disorders or not.

Although PSG is regarded as a gold rule for sleep research, it also has many drawbacks. For example, people are normally subject to the equipments which are used for collecting data so that they are unlikely to conduct a PSG test at home or even cannot collect reliable data. In addition to this, PSG scoring also usually varies from laboratory to laboratory. Because of those drawbacks, it is obvious that we cannot implement the whole PSG standard on our device directly. Therefore we refer to some other researches, like Sleep Evaluation by Actigraphy and A novel approach using actigraphy to quantify the level of disruption of sleep by in-home ploysomnography etc, and combine those references, then, come up with a assessment.
Here, assessment as follows:

* Sleep latency (20 minutes or less), the moment an individual slept since the lights were switched off.

* Sleep efficiency, which is the minutes of total sleep divided by the minutes spent on bed. In normal cases, it falls between 85%-90%.

* Sleep stages, which are based on the data coming from various kinds of sensors, like sound sensors, light sensors, motion sensors as well as heart rhythm sensors.

# data visualization example
By using mysql database, the local Raspberry Pi can connect and push the data to the database, and the website can grabbing and showing the data in properly way to the user.

The site is based on *Ubuntu Linux* system, *Apache* server, *MySQL* database and most of pages are wrriten by *HTML*, *CSS*, *JavaScript* and *PHP*. *jQuery* and *Chart.js* are also being used for efficiency and goodlooking.

Here is an example page for what data will be showing: http://78.141.235.21/rtshow.html

~~It may took around 5 seconds to showing, better viewing implementation is developing by team member.~~

Better view has been implemented. the page will showing data when the page finished load and update the data every 5 seconds. Chart will transform smoothly.

![view-example1](https://github.com/UofG-RTEP-Team25/SleepQualityEvaluationRPi/blob/main/Documents/img/view-example1.png?raw=true)


<!-- CONTACT -->
## contact us

Zhongju Zhu     -2547408Z@student.gla.ac.uk

Shengtao Zhong  -2586232Z@student.gla.ac.uk

Yangbolun Zhou  -2515369Z@student.gla.ac.uk

* [Twitter](https://twitter.com/jianzha47918304/status/1381001029836226560?s=21) 

* [Youtube](https://www.youtube.com/watch?v=cMlTJh96JMU) 

* [Instagram](https://www.instagram.com/glasgowteam15/) 


Project Link: [ https://github.com/UofG-RTEP-Team25/SleepQualityEvaluationRPi]( https://github.com/UofG-RTEP-Team25/SleepQualityEvaluationRPi)



# references
[Sleep Evaluation by Actigraphy .pdf](https://github.com/UofG-RTEP-Team25/SleepQualityEvaluationRPi/files/6055883/Sleep.Evaluation.by.Actigraphy.pdf)

[A novel approach using actigraphy to quantify the level of disruption of sleep by in-home polysomnography - the MrOS Sleep Study Sleep disruption by polysomnography.pdf](https://github.com/UofG-RTEP-Team25/SleepQualityEvaluationRPi/files/6055884/A.novel.approach.using.actigraphy.to.quantify.the.level.of.disruption.of.sleep.by.in-home.polysomnography.-.the.MrOS.Sleep.Study.Sleep.disruption.by.polysomnography.pdf)

https://emedicine.medscape.com/article/1188764-overview

https://web.archive.org/web/20070929205410/http://www.sleep-tests.co.uk/polysomnography.php

https://github.com/sparkfun/SparkFun_MAX3010x_Sensor_Library

[i2c_bus_specification_1995.pdf](https://github.com/UofG-RTEP-Team25/SleepQualityEvaluationRPi/files/6292281/i2c_bus_specification_1995.pdf)




<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/badge/CONTRIBUTORS-3-green
[contributors-url]: https://github.com/UofG-RTEP-Team25/SleepQualityEvaluationRPi/graphs/contributors
[forks-shield]: https://img.shields.io/badge/FORKS-blue
[forks-url]: https://github.com/UofG-RTEP-Team25/SleepQualityEvaluationRPi/network/members
[stars-shield]: https://img.shields.io/badge/STARS-red
[stars-url]: https://github.com/UofG-RTEP-Team25/SleepQualityEvaluationRPi/stargazers
[issues-shield]: https://img.shields.io/badge/ISSUES-yellow
[issues-url]: https://github.com/UofG-RTEP-Team25/SleepQualityEvaluationRPi/issues
[license-shield]: https://img.shields.io/badge/LICENSE-MIT-green
[license-url]: https://github.com/UofG-RTEP-Team25/SleepQualityEvaluationRPi/blob/main/LICENSE
[product-screenshot]: images/screenshot.png
