<script>
    import Button from "./lib/Button.svelte";
    import Card from "./lib/Card.svelte";
    import CardBody from "./lib/CardBody.svelte";
    import CardFooter from "./lib/CardFooter.svelte";
    import CardTitle from "./lib/CardTitle.svelte";
    import InputLabel from "./lib/InputLabel.svelte";

    let result = 0
    let name = 'renan' 
    let height, weight;

    const sendButton = () => {
      result = +Number(weight / (height * height)).toFixed(2)
    }

</script>

<Card>
  <CardTitle title='BMI App'/>
  <CardBody>
    <form action="">
      <InputLabel name="name" type="text" bind:v={name}/>
      <InputLabel name="weight" type="number" bind:v={weight}/>
      <InputLabel name="height" type="number" bind:v={height}/>
      
      <Button innerText="Calculate" func={sendButton}/>
    </form>

    <section>
      <h4>BMI: {result}</h4>
    </section>
  </CardBody>
  <CardFooter description="Renan Lira@2020"/>
</Card>

<style>
  
  form {
    display: flex;
    width: 100%;
    height: 60%;
    flex-direction: column;
    gap: 1.3rem; 
    margin-top: 1.3rem;
  }

  section {
    flex: 1;
    font-size: 2.2rem;
    display: flex;
    flex-direction: column;
    justify-content: center;
  }
</style>
