
### README
---
Hello, I am a computer science student and mainly program in C and C++.

![](https://komarev.com/ghpvc/?username=pscieszka&color=blueviolet)


### Technologies

  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=git,github,c,cpp,cs,dotnet,html,css,py" />
  </a>


### Projects
---
I am currently working on a password manager project that utilizes the OpenSSL library.

The password manager is a secure application that allows users to store and manage their passwords. The application uses the OpenSSL library for encryption and decryption of user data. The project is written in C++.

### Leetcode
![](https://badges.peiyuan.ch/leetcode/laylow28inches/solved)\
![](https://badges.peiyuan.ch/leetcode/laylow28inches/solved?difficulty=easy)\
![](https://badges.peiyuan.ch/leetcode/laylow28inches/solved?difficulty=medium)\
![](https://badges.peiyuan.ch/leetcode/laylow28inches/solved?difficulty=hard)

<h2>LeetCode Problem Status</h2>
<div class="problem-status">
  <div class="problem-status-bar">
    <div class="problem-status-bar-fill" id="problem-status-easy"></div>
  </div>
  <div class="problem-status-bar">
    <div class="problem-status-bar-fill" id="problem-status-medium"></div>
  </div>
  <div class="problem-status-bar">
    <div class="problem-status-bar-fill" id="problem-status-hard"></div>
  </div>
</div>

<script>
const username = 'laylow28inches}'; 
const url = `https://leetcode.com/api/problems/all/?username=${username}`;

fetch(url)
  .then(response => response.json())
  .then(data => {
    const problems = data.stat_status_pairs;
    let easySolved = 0;
    let mediumSolved = 0;
    let hardSolved = 0;
    problems.forEach(problem => {
      if (problem.status === 'ac') {
        if (problem.difficulty.level === 1) {
          easySolved++;
        } else if (problem.difficulty.level === 2) {
          mediumSolved++;
        } else if (problem.difficulty.level === 3) {
          hardSolved++;
        }
      }
    });
    const total = easySolved + mediumSolved + hardSolved;
    const easyPercent = (easySolved / total) * 100;
    const mediumPercent = (mediumSolved / total) * 100;
    const hardPercent = (hardSolved / total) * 100;
    document.getElementById('problem-status-easy').style.width = `${easyPercent}%`;
    document.getElementById('problem-status-medium').style.width = `${mediumPercent}%`;
    document.getElementById('problem-status-hard').style.width = `${hardPercent}%`;
  })
  .catch(error => console.log(error));
</script>

<style>
.problem-status {
  display: flex;
  justify-content: space-between;
}

.problem-status-bar {
  width: 100px;
  height: 20px;
  background-color: #ddd;
  border-radius: 10px;
  overflow: hidden;
  margin-right: 10px;
}

.problem-status-bar-fill {
  height: 100%;
}

#problem-status-easy {
  background-color: #28a745;
}

#problem-status-medium {
  background-color: #ffc107;
}

#problem-status-hard {
  background-color: #dc3545;
}
</style>
### Contact
---
You can reach me at piotr.scieszka02@gmail.com or through my GitHub profile.
