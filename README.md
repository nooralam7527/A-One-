// A1 Fashion Website - Future Ready

import React from "react"; import { BrowserRouter as Router, Routes, Route } from "react-router-dom"; import { Home } from "./pages/Home"; import { Shop } from "./pages/Shop"; import { Product } from "./pages/Product"; import { Cart } from "./pages/Cart"; import { Login } from "./pages/Login"; import { Register } from "./pages/Register"; import { About } from "./pages/About"; import { Contact } from "./pages/Contact"; import { Blog } from "./pages/Blog"; import { Navbar } from "./components/Navbar"; import { Footer } from "./components/Footer"; import "./App.css";

function App() { return ( <Router> <Navbar /> <main className="min-h-screen p-4 bg-gray-50"> <Routes> <Route path="/" element={<Home />} /> <Route path="/shop" element={<Shop />} /> <Route path="/product/:id" element={<Product />} /> <Route path="/cart" element={<Cart />} /> <Route path="/login" element={<Login />} /> <Route path="/register" element={<Register />} /> <Route path="/about" element={<About />} /> <Route path="/contact" element={<Contact />} /> <Route path="/blog" element={<Blog />} /> </Routes> </main> <Footer /> </Router> ); }

export default App;
