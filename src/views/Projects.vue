<template>
    <main class="projects">
        <h4>Welcome to my personal project page</h4>
            <section class="project-container">
                <div class="project-list">
                    <h3>Projects I have done</h3>
                    <div class="project-card">
                        <img class="image" src="../assets/todo5.jpg" alt="">
                            <div class="proj-descrip">
                                <h3>Rocket Game</h3>
                                <p>I developed this Rocket Game in my first C++ class at Boston University</p>
                            </div>
                    </div>
                    <div class="project-card">
                        <img class="image" src="../assets/todo6.jpg" alt="">
                            <div class="proj-descrip">
                                <h3>Fitness Application</h3>
                                <p>This was a group project for my Software Engineering class at Boston University</p>
                                <a href="https://github.com/CS673Spring" target="_blank">Fitness App</a>
                            </div>
                    </div>
                    <div class="project-card">
                        <img class="image" src="../assets/todo7.jpg" alt="">
                            <div class="proj-descrip">
                                <h3>Educational Website</h3>
                                <p>This was a group project developed in my Agile Development class at Boston University. It was created using wordpress</p>
                                <a href="https://cs601691078774.wordpress.com/" target="_blank">Ace Education</a>
                            </div>
                    </div>
                    <div class="project-card">
                        <img class="image" src="../assets/todo8.jpg" alt="">
                            <div class="proj-descrip">
                                <h3>Personal Website</h3>
                                <p>The site you are on now!</p>
                            </div>
                    </div>
                </div>
                <div class="project-list">
                    <h3>Projects I am working towards</h3>
                    <div class="project-card">
                        <img class="image" src="../assets/todo1.jpg" alt="">
                            <div class="proj-descrip">
                                <h3>Chess Engine</h3>
                                <p>A chess engine analyzes the chess board and suggests the best next move. Besides that, it might serve as an opponent in playing with the computer. Implement the next generation AI-powered chess engine.</p>
                            </div>
                    </div>
                    <div class="project-card">
                        <img class="image" src="../assets/todo2.jpg" alt="">
                            <div class="proj-descrip">
                                <h3>Chat Bot</h3>
                                <p>A chatbot or chatterbot is a software application used to conduct an on-line chat conversation via text or text-to-speech, in lieu of providing direct contact with a live human agent. A chatbot is a type of software that can help customers by automating conversations and interact with them through messaging platforms. </p>
                            </div>
                    </div>
                    <div class="project-card">
                        <img class="image" src="../assets/todo3.jpg" alt="">
                            <div class="proj-descrip">
                                <h3>P2P Messaging Application</h3>
                                <p>Implement an application for chatting with a friend. The challenge is to make it in a way that omits a centralized server and initiates a direct connection between two chat clients.</p>
                            </div>
                    </div>
                    <div class="project-card">
                        <img class="image" src="../assets/todo4.jpg" alt="">
                            <div class="proj-descrip">
                                <h3>Dropbos Clone</h3>
                                <p>Dropbox is a file sharing application. Consists of clients for almost all operating systems, including Android and iOS. It also has a huge backend. Design and implement your own version of a file sharing application that works at least for 10 users and provides 100 Mb of space to each of them. Implement both the server and the client (at least for one OS).</p>
                            </div>
                    </div>
                </div>
            </section>
            <div>
                <h4>Personal Project Video on Security</h4>
                <iframe class="video" src="https://www.youtube.com/embed/0OrVEeX7Z5s" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
            </div> 
    </main>
</template>

<script>


</script>

<style>

.projects {
    display: flex;
    flex-direction: column;
    align-items: center;
       animation: fadeInAnimation ease .5s;
            animation-iteration-count: 1;
            animation-fill-mode: forwards;
        }
        @keyframes fadeInAnimation {
            0% {
                opacity: 0;
            }
            100% {
                opacity: 1;
            }
}


.projects h4 {
    display: flex;
    align-content: center;
    font-family: 'Fira sans', sans-serif;
    font-size: 1.4rem;
    margin-bottom: 10px;

}

.project-container {
    display: flex;
    flex-direction: row;
    width: 97rem;
}

.project-list {
    width: 700px;
    margin: 50px auto;
    padding: 10px 5px;
    border-radius: 10px;
    background:  rgb(202, 202, 202, 0.3);
     -webkit-box-shadow: 0 1px 3px rgba(0, 0, 0, 0.12),0 1px 2px rgba(0, 0, 0, 0.24);
    box-shadow: 0 1px 3px rgba(0, 0, 0, 0.12), 0 1px 2px rgba(0, 0, 0, 0.24);  
}

.project-card {
    border: rgb(84, 89, 95);
    border-style: solid;
    border-width: 3px;
    border-radius: 5px;
    margin: 5px;
    height: 400px;
    position: relative;
    display: flex;
    flex-direction: row;
}

.project-card p h3 {
    display: flex;
    align-items: center;
    margin: auto 15px;
}

.proj-descrip {
    display: flex;
    flex-direction: column;
    align-content: center;
    margin-top: 11rem;

}

.image {
    max-width: 270px;
    margin: 19px;
    height: 360px;
    align-content: center;
    object-fit: cover;
    border-radius: 5px;
}

.video {
    display: flex;
    margin: auto;
    width:560px; 
    height:325px; 
}

</style>