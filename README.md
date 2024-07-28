// screens/HomeScreen.js
import React, { useState, useEffect } from 'react';
import { View, Text, Button, TextInput } from 'react-native';
import axios from 'axios';

const HomeScreen = ({ navigation }) => {
    const [balance, setBalance] = useState(0);
    const [toUsername, setToUsername] = useState('');
    const [amount, setAmount] = useState('');

    useEffect(() => {
        // Fetch balance from server
    }, []);

    const handleTransfer = async () => {
        try {
            // Perform transfer
        } catch (error) {
            console.error(error);
        }
    };

    return (
        <View>
            <Text>Balance: {balance}</Text>
            <TextInput placeholder="Recipient" value={toUsername} onChangeText={setToUsername} />
            <TextInput placeholder="Amount" value={amount} onChangeText={setAmount} />
            <Button title="Transfer" on
