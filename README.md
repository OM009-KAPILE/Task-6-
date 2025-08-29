import React from "react";

function ProfileCard({ name, role, image }) {
  return (
    <div style={styles.card}>
      <img src={image} alt={name} style={styles.image} />
      <h2>{name}</h2>
      <p>{role}</p>
    </div>
  );
}

function App() {
  return (
    <div style={styles.container}>
      <h1>Profile Cards</h1>
      <ProfileCard 
        name="Om Kpile" 
        role="Frontend Developer" 
        image="https://via.placeholder.com/150"
      />
      <ProfileCard 
        name="Aarav Sharma" 
        role="Backend Developer" 
        image="https://via.placeholder.com/150/0000FF/FFFFFF"
      />
    </div>
  );
}

const styles = {
  container: {
    fontFamily: "Arial, sans-serif",
    textAlign: "center",
    padding: "20px"
  },
  card: {
    border: "1px solid #ddd",
    borderRadius: "12px",
    width: "200px",
    margin: "10px auto",
    padding: "15px",
    boxShadow: "0 4px 8px rgba(0,0,0,0.1)"
  },
  image: {
    width: "100%",
    borderRadius: "50%"
  }
};

export default App;
