<template>
    <div id="about">
        <h1 class="title">About</h1>
        <div class="about-me">
            <img src="../assets/images/background.jpg" alt="My Image">
            <div class="info">
                <h3>Fullstack JavaScript and Mobile App Developer</h3>
                <p>My Personal Informations</p>
                <div class="personal-info">
                    <p><span>Birthday:</span> 15 Nov 2000</p>
                    <p><span>Email:</span> eabebe91@gmail.com</p>
                    <p><span>Phone:</span> +251 964643164</p>
                    <p><span>City:</span> Gondar, Amhara, Ethiopia</p>
                    <p><span>Age:</span> 21</p>
                </div>


            </div>
        </div>
    </div>
</template>

<style scoped>
#about {
    margin: 1.5rem;
}

.title {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-transform: uppercase;
}

.title::after {
    content: '';
    margin-top: 1rem;
    margin-bottom: 2rem;
    display: block;
    height: 4px;
    width: 5rem;
    background-color: #34b7a7;
    border-radius: 5px;
}

.about-me {
    display: flex;
    gap: 1rem;
}

.about-me img {
    width: 40%;
}

.info {
    display: flex;
    flex-direction: column;
    gap: 1rem;
    align-items: center;
}

.info > p{
    font-weight: 600;

}

.personal-info {
    /* flex-grow: 2; */
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 1rem;
}

@media (max-width: 850px) {

    #about {
        margin: 2rem 5vw;
    }
    .about-me {
        flex-direction: column;
    }

    .about-me img {
        width: 100%;
    }
}

@media (max-width: 550px) {
    .personal-info {
        grid-template-columns: 1fr;
        gap: 1rem;
    }
}
</style>