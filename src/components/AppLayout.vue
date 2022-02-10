 <template>
<div class ="layout">
  <header>
    <slot name="header">header</slot>
    </header>
    <main>
      <slot/>
      </main>
      <footer>
        <slot name="footer">footer</slot>
        </footer>
        </div>
</template>

<script>
export default {

};
</script>

<style scoped>
header,footer {
  color: white;
  display: flex;
  align-items: center;
  padding: 0.25rem 0.5rem;
  border: none;
  
  font-weight: bold;
  background-color: #41b883;
  border-radius: 0.25rem;
  line-height: 1.5;
  margin: 10px;
}
</style> 

