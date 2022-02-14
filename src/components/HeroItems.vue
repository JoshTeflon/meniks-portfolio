<script>
    import Button from './Button.vue'

	export default {
        name: "HeroItems",
        components: {
            Button,
        },
        data() {
            return {
                emailBg: '#3394cb',
                cvBg: '#33cb98',
            }
        }
	}
</script>

<template>
    <div class="hero--items">
        <h1 class="hero--intro">Hello, I'm <span class="mk--name">Moses Enikele</span></h1>
        <h2 class="hero--career">A Researcher & IT Consultant </h2>
        <p class="hero--summary">I am into Project Management, Human Resource Management and Customer Service & Relationship Management.</p>
        <div class="cta-btn--group">
            <a class="cta-btn--1" href="mailto: consultantsemi@gmail.com?subject=RESEARCHER & IT CONSULTANT&body=Hello Moses Enikele," target="_blank" rel="noopener noreferrer">
                <Button action="Email me" :background="emailBg"  />
            </a>
            <a class="cta-btn--2" href="../assets/ENIKELE Moses ISEGHOSIME Resume.docx" target="_blank" rel="noopener noreferrer">
                <Button action="Download CV" :background="cvBg"  />
            </a>
        </div>
    </div>
</template>

<style scoped>
    .hero--items .hero--intro {
        font-size: 2rem;
        font-weight: 400;
    }
    .hero--items .hero--career {
        font-size: 2.2rem;
        font-weight: 500;
        letter-spacing: 0.05rem;
        margin: 0.75rem 0;
    }
    .hero--items .hero--summary {
        font-size: 1rem;
        font-weight: 400;
    }
    .hero--items .mk--name {
        color: var(--mk-c-blue-1);
        font-size: 2rem;
        font-weight: 700;
    }
    .hero--items .cta-btn--group {
        display: flex;
        align-items: center;
        margin-top: 1.5rem;
    }

    .hero--items .cta-btn--2 {
        margin-left: 2rem;
    }

    @media screen and (min-width: 640px) {
        .hero--items .hero--intro {
            font-size: 2rem;
        }

        .hero--items .mk--name {
            font-size: 2rem;
        }

        .hero--items .hero--career {
            font-size: 2.25rem;
        }
    }

    @media screen and (min-width: 1024px) {
        .hero--items .hero--summary {
            width: 90%;
        }
    }

    @media screen and (min-width: 1200px) {
        .hero--items .hero--summary {
            width: 80%;
        }
    }
</style>