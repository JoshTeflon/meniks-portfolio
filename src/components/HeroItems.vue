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
            <a class="cta-btn--2" href="../assets/ENIKELE Moses ISEGHOSIME Resume.pdf" download>
                <Button action="Download CV" :background="cvBg"  />
            </a>
        </div>
    </div>
</template>

<style scoped>
    .hero--items {
        width: 100%;
        margin: 2rem auto;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }
    .hero--items .hero--intro {
        font-size: 2rem;
        font-weight: 400;
    }
    .hero--items .hero--career {
        font-size: 1.75rem;
        font-weight: 700;
        letter-spacing: 0.05rem;
        margin: 0.75rem 0;
    }
    .hero--items .hero--summary {
        font-size: 1.25rem;
        font-weight: 400;
        /* width: 100%; */
        line-height: 150%;
        text-align: center;
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
        .hero--items {
            display: block;
        }

        .hero--items .hero--intro {
            font-size: 2rem;
        }

        .hero--items .mk--name {
            font-size: 2rem;
        }

        .hero--items .hero--summary {
            text-align: left;
        }

        .hero--items .hero--career {
            font-size: 2.4rem;
        }
    }

    @media screen and (min-width: 1024px) {
        .hero--items .hero--summary {
            width: 100%;
        }
    }

    @media screen and (min-width: 1200px) {
        .hero--items .hero--summary {
            width: 100%;
        }
    }
</style>