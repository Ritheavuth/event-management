<template>
  <div class="root-div">
        
        <div class="left side">
            <header>
                <h1>Create your <br> Event here</h1>
            </header>
            <section>
                <img src="src\assets\test.jpeg" alt="">
            </section>
        </div>

        <div class="right side">

            <form action="" method="get">
                <section id="event-title">
                    <label>Event Title</label>
                    <input type="text" placeholder="Title">
                </section>
                
                <section id="event-type">
                    <label>Event Type <span>(optional)</span></label>
                    <select name="" id="">
                        <option value="Private" class="type">Private</option>
                        <option value="Corporate" class="type">Corporate</option>
                        <option value="Charity" class="type">Charity</option>
                    </select>
                </section>

                <section id="date">
                    <label>Date</label>
                    <div>
                        <input type="text" class="date"><label>/</label>
                        <input type="text" class="date"><label>/</label>
                        <input type="text" class="date">
                    </div>
                    
                </section>
                
                <section id="location">
                    <label>Location</label>
                    <input type="text" placeholder="Location">
                </section>

                <section id="event-desc">
                    <label>Event Description</label>
                    <input type="text" placeholder="Event Description...">
                </section>

                <section id="event-img">
                    <label>Event Image</label>
                    <input type="file">
                </section>

                <section id="ticket-type">
                    <label>Ticket Type</label>
                    <div>
                        <section class="ticket-type--name">
                            <label>Name</label>
                            <input type="text">
                        </section>
    
                        <section class="ticket-type--price">
                            <label>Price</label>
                            <input type="text">
                        </section>
    
                        <section class="ticket-type--no">
                            <label>No.</label>
                            <input type="text">
                        </section>
                    </div>
                </section>

            </form>

        </div>
        

    </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.root-div {
    margin: 0 auto;
    width: 900px;
    height: 630px;
    display: flex;
    flex-direction: row;
}

.root-div .side {
    width:50%;
    height: 100%;
}

.root-div .left {
    display: flex;
    flex-direction: column;
}

.root-div .left header {
    background-color: indigo;
    width: 100%;
    height: 20%;
    text-align: center;
    color: #fff;
    font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
}

.root-div .left section {
    height: 80%;
    width: 100%;
}

.root-div .left section img {
    height: 100%;
    width: 100%;
}

.root-div .right{
    color: blue;
}

.root-div .right form {
    display: flex;
    flex-direction: column;
    height: auto;
    width: 400px;
    margin: 15px 25px;
}

.root-div .right form {
    justify-content: space-evenly;
}

.root-div .right form input, select {
    width: 96%;
    height: 30px;
    margin-bottom: 20px;
}

.root-div .right #date {
    display: flex;
    flex-direction: column;
}

.root-div .right #date div {
    display: flex;
    flex-direction: row;
    font-size: 25px;
}

.root-div .right #date div input {
    width: 28%;
}

.root-div .right #date div label {
    margin: 0 1%;
}

.root-div .right #event-desc input {
    height: 100px;
}

.root-div .right #ticket-type {
    display: flex;
    flex-direction: column;
}

.root-div .right #ticket-type div {
    display: flex;
    flex-direction: row;
    justify-content: space-evenly;
}

.root-div .right #ticket-type div section {
    display: flex;
    flex-direction: column;
    margin: 0 2.2%;   
}

.root-div .right #ticket-type div .ticket-type--name {
    width: 40%;
}

.root-div .right #ticket-type div .ticket-type--name input {
    width: 100%;
}

.root-div .right #ticket-type div .ticket-type--price {
    width: 30%;
}

.root-div .right #ticket-type div .ticket-type--price input {
    width: 100%;
}

.root-div .right #ticket-type div .ticket-type--no {
    width: 10%;
}

.root-div .right #ticket-type div .ticket-type--no input {
    width: 100%;
}
</style>
