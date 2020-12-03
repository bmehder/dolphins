<script>
  // Layout Components
  import Header from "./Layouts/Header.svelte";
  import Section from "./Layouts/Section.svelte";
  import Grid from "./Layouts/Grid.svelte";
  import Flex from "./Layouts/Flex.svelte";
  import Footer from "./Layouts/Footer.svelte";

  // UI Components
  import Timeline from "./UI/Timeline.svelte";
  import Tabs from "./UI/Tabs.svelte";
  import FancyCard from "./UI/FancyCard.svelte";
  import Form from "./UI/Form.svelte";
  import Blockquote from "./UI/Blockquote.svelte";
  import Hero from "./UI/Hero.svelte";
  import Button from "./UI/Button.svelte";
  import Fetcher from "./UI/Fetcher.svelte";
  import Animation from "./UI/Animation.svelte";
  import Gooey from "./UI/Gooey.svelte";
  import CTA from "./UI/CTA.svelte";
  import Typewriter from "./UI/Typewriter.svelte";
  import Card from "./UI/Card.svelte";

  // Data Stores
  import { tennis } from "./Data/tennis.js";
  import { tabData } from "./Data/tabData.js";
</script>

<div class="wrapper">
  <Header background="linear-gradient(to right, #606c88, #3f4c6b)" />
  <main>
    <Hero
      background="https://source.unsplash.com/random/"
      title="So long, and thanks for all the fish.">
      <Button uppercase reflection shadow background="#f06">Make My Day</Button>
    </Hero>

    <Section
      background="white"
      padding="4em 2em"
      title="Lorem Ipsum Dolor"
      titleColor="#f06">
      <!-- <h3>Lorem Ipsum</h3> -->
      <Grid columns="1fr 1fr" gap="2em">
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. A consectetur
          laudantium libero? Omnis vel nostrum culpa nesciunt facilis magni rem!
          Nisi corrupti, adipisci a similique aliquam cum vero non nam, eveniet
          libero ratione neque harum amet asperiores reiciendis sequi atque
          temporibus ad blanditiis iusto quae? Earum, dolorum iure. Animi,
          magnam.
        </p>

        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. A consectetur
          laudantium libero? Omnis vel nostrum culpa nesciunt facilis magni rem!
          Nisi corrupti, adipisci a similique aliquam cum vero non nam, eveniet
          libero ratione neque harum amet asperiores reiciendis sequi atque
          temporibus ad blanditiis iusto quae? Earum, dolorum iure. Animi,
          magnam.
        </p>
      </Grid>
      <Blockquote shadow>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. A consectetur
        laudantium libero?
      </Blockquote>
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. A consectetur
        laudantium libero? Omnis vel nostrum culpa nesciunt facilis magni rem!
        Nisi corrupti, adipisci a similique aliquam cum vero non nam, eveniet
        libero ratione neque harum amet asperiores reiciendis sequi atque
        temporibus ad blanditiis iusto quae? Earum, dolorum iure. Animi, magnam.
        corrupti, adipisci a similique aliquam cum vero non nam, eveniet libero
        ratione neque harum amet asperiores reiciendis sequi atque temporibus ad
        blanditiis iusto quae? Earum, dolorum iure.
      </p>
    </Section>

    <Section
      title="Wimbledon Champions"
      titleColor="white"
      padding="2em"
      background="linear-gradient(to right, #606c88, #3f4c6b)">
      <Timeline data={tennis} />
    </Section>

    <Section
      padding="2em 2em 4em"
      background="white"
      title="Fancy Cards"
      titleColor="#f06">
      <Grid columns="1fr 1fr 1fr" place="center" gap="4em">
        <FancyCard
          metal
          raise
          ribbon
          content="adipisci a similique aliquam cum vero non nam, eveniet libero
        ratione neque harum amet asperiores reiciendis sequi atque temporibus ad
        blanditiis iusto quae?" />
        <FancyCard
          metal
          raise
          ribbon
          content="adipisci a similique aliquam cum vero non nam, eveniet libero
        ratione neque harum amet asperiores reiciendis sequi atque temporibus ad
        blanditiis iusto quae?" />
        <FancyCard
          metal
          raise
          ribbon
          content="adipisci a similique aliquam cum vero non nam, eveniet libero
        ratione neque harum amet asperiores reiciendis sequi atque temporibus ad
        blanditiis iusto quae?" />
      </Grid>
    </Section>

    <Hero
      background="https://source.unsplash.com/random/?1"
      height="600px"
      padding="2em"
      title="You won't believe this."
      color="#fff" />

    <Section padding="4em 2em">
      <Flex justify="space-around" align="center">
        <Card>
          <h3>Heading</h3>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Enim, quasi
          quam. Expedita temporibus doloremque reiciendis earum beatae, soluta
          dignissimos ut debitis quo nemo, cumque quisquam, iusto necessitatibus
          natus dolorem odit.
          <Button>Click Me</Button>
        </Card>
        <Card>
          <h3>Heading</h3>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Enim, quasi
          quam. Expedita temporibus doloremque reiciendis earum beatae, soluta
          dignissimos ut debitis quo nemo, cumque quisquam, iusto necessitatibus
          natus dolorem odit.
          <Button>Click Me</Button>
        </Card>
        <Card>
          <h3>Heading</h3>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Enim, quasi
          quam. Expedita temporibus doloremque reiciendis earum beatae, soluta
          dignissimos ut debitis quo nemo, cumque quisquam, iusto necessitatibus
          natus dolorem odit.
          <Button>Click Me</Button>
        </Card>
      </Flex>
    </Section>

    <Section
      background="#ff9f55"
      title="Only 4 Simple Steps"
      titleColor="white"
      padding="4em 2em">
      <Grid columns="1fr 2fr" gap="3em" place="end">
        <FancyCard
          ribbon
          metal
          title="It's Easy!"
          content="Lorem ipsum dolor sit, amet consectetur adipisicing elit."
          center />
        <Tabs data={tabData} />
      </Grid>
    </Section>

    <Section
      background="#3f4c6b"
      padding="2em"
      title="Contact Us"
      titleColor="white">
      <Form
        titleColor="white"
        buttonColor="#f06"
        buttonText="Send Message"
        buttonTextColor="white" />
    </Section>

    <Section background="#606c88" padding="2em">
      <Typewriter phrase="So long, and thanks for all the fish." />
    </Section>
  </main>
  <Footer background="#3f4c6b">
    &copy; 2021 Brad Mehder. All rights reserved.
  </Footer>
</div>

<style>
  :global(body) {
    background: linear-gradient(to right, #606c88, #3f4c6b);
    font-family: "Open Sans", sans-serif;
  }
  .wrapper {
    display: grid;
    grid-template-rows: auto 1fr auto;
    min-height: 100vh;
  }
</style>
