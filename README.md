<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>NCTO_FAQs</title>
<style>
  body {
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    background-color: #ffffff;
    font-family: 'Arial', sans-serif;
  }

  .faq-container {
    max-width: 800px;
    width: 90%;
    margin: 0 auto;
    padding: 30px;
    background-color: #fff;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    overflow: hidden;
  }

  .banner {
    color: #fff;
    padding: 10px 0;
    text-align: center;
    border-top-left-radius: 10px;
    border-top-right-radius: 10px;
  }

  .logo {
    max-width: 120px;
    margin-bottom: 10px;
  }

  .social-links {
    display: flex;
    justify-content: center;
  }

  .social-links a {
    margin: 0 10px;
    text-decoration: none;
    color: #4caf50;
    font-weight: bold;
    transition: color 0.3s ease;
    background-color: #fff;
    padding: 8px 16px;
    border-radius: 20px;
    border: 2px solid #4caf50;
  }

  .social-links a:hover {
    color: #ffcd00;
    border-color: #ffcd00;
  }

  .question {
    cursor: pointer;
    font-weight: 700;
    margin-bottom: 20px;
    color: #00cc00;
    transition: color 0.3s ease;
  }

  .question:hover {
    color: #FDDC21;
  }

  .answer {
    display: none;
    margin-bottom: 30px;
    color: #666;
    font-size: 16px;
    line-height: 1.5;
  }

  .answer.show {
    display: block;
    animation: fadeIn 0.5s ease;
  }

  @keyframes fadeIn {
    from {
      opacity: 0;
      transform: translateY(-10px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }
</style>
</head>
<body>

<div class="banner">
  <img src="https://scontent.fabv2-2.fna.fbcdn.net/v/t39.30808-1/386252141_706908961464404_2936806290879949661_n.jpg?stp=c13.3.194.194a_dst-jpg_p200x200&_nc_cat=111&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeEtFH62zfHo7frY-tw5PDB79KMZqKLWXcf0oxmootZdxw8v4HAFfb-KsAry6WNF1u9qCcoFImuK4QzPPB1_-SWy&_nc_ohc=4YbJv52kABwAX-TEEyC&_nc_ht=scontent.fabv2-2.fna&oh=00_AfC3VProHFy3ubBmQW3C0DNh7WLQ2VCn0mrgNgKjh_4Dgw&oe=66118EBC" alt="Your Logo">
  <div class="social-links">
    <a href="https://web.facebook.com/betadoncome" target="_blank">Facebook</a>
    <a href="https://twitter.com/RHCCT25k" target="_blank">Twitter</a>
    <a href="#" target="_blank">Instagram</a>
  </div>
</div>

<div style="text-align: center; margin-top: 20px;">
 <p> <h2>Frequently Asked Questions</h2> </p>
</div>

<div class="faq-container">
  <div class="faq-content">
    <div class="question" onclick="toggleAnswer('q1')">What is the National Social Safety-nets Project - Scale Up (NASSP-SU) all about? </div>
    <div class="answer" id="q1">The NASSP-SU is a follow-on operation to the NASSP, and intends to build on and scale up the existing delivery system to provide shock responsive safety nets and to extend regular social assistance to the poor and vulnerable. </p>The project is designed to offer time-limited cash transfers in response to recent shocks (food price inflation) in rural as well as urban areas. The project will also extend the duration of support to the current beneficiaries of NASSP regular cash transfer program - yet to receive 18 cycles of benefits.</div>

    <div class="question" onclick="toggleAnswer('q2')">The Project Development Objective is?</div>
    <div class="answer" id="q2">The broad objective of the project is to expand coverage of shock responsive safety net support among the poor and vulnerable and strengthen the national safety net delivery system.</div>

    <div class="question" onclick="toggleAnswer('q3')">Is the programme a palliative?</div>
    <div class="answer" id="q3">No, it is aimed at cushioning the economic hardship being experienced by identified rural and urban households due to the ongoing economic reforms of Government.</div>

 <div class="question" onclick="toggleAnswer('q4')">Who are the beneficiaries of the NASSP Scale Up?</div>
    <div class="answer" id="q4">Beneficiaries of NASSP SU are sourced from the National Social Register targeting poor and vulnerable rural households and the Rapid Response Register targeting poor and vulnerable urban households.</div>

 <div class="question" onclick="toggleAnswer('q5')">How do I benefit in this beautiful initiative?</div>
    <div class="answer" id="q5">Firstly, you must be identified and registered in the National Social Register, Rapid Response Register and other acceptable Registers of poor and vulnerable households in Nigeria. </p>You will them be enroled with your account details for direct payment to your account.</div>

 <div class="question" onclick="toggleAnswer('q6')">How much will I benefit?</div>
    <div class="answer" id="q6">If you are eligible and enrolled, you will benefit N75,000 direct payment to your account i.e. N25,000 per month.</div>

 <div class="question" onclick="toggleAnswer('q7')">How long will I benefit?</div>
    <div class="answer" id="q7">If you are eligible and enrolled, you will benefit direct payment to your account for three months.</div>

 <div class="question" onclick="toggleAnswer('q8')">Can I benefit without a National Identification Number (NIN)?</div>
    <div class="answer" id="q8">You can NEVER benefit without a NIN or BVN.</div>

 <div class="question" onclick="toggleAnswer('q9')">I am a beneficiary of the Household Uplifting Programme HUP-CCT, Will I benefit?</div>
    <div class="answer" id="q9">You will not benefit from NASSP SU if you have received N10,000 (ten thousand Naira) 18 times during NASSP (HUP-CCT).</div>

  </div>
</div>

<script>
function toggleAnswer(id) {
  var allAnswers = document.querySelectorAll('.answer');
  allAnswers.forEach(function(answer) {
    if (answer.id === id) {
      answer.classList.toggle('show');
    } else {
      answer.classList.remove('show');
    }
  });
}
</script>

</body>
</html>
