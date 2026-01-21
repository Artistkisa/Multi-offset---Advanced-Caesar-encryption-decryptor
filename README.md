# Multi-offset---Advanced-Caesar-encryption-decryptor
This expanded version of the Caesar Code enhances the complexity and security of the traditional Caesar Code by introducing dynamic offset sequences and displacement steps. Each word uses a different displacement pattern when encrypting, making the encryption results more diverse and difficult to crack.

Encryption Process:

Select an offset sequence: Choose an offset sequence for each word (e.g. (fictional) aba": [11, 3, 8, 18, 9]), which determines how the letters are displaced.

Apply Displacement Steps: For each letter in the word, apply the displacement steps in the offset sequence in turn. If the word length exceeds the length of the step array, those steps are cycled.

Generate ciphertext: Each encrypted word is followed by a corresponding offset sequence code for identification during decryption.

Handling Non-Alphabetic Characters: Non-alphabetic characters are not involved in encryption, leaving them as is.

Features: Dynamic encryption makes each word use an independent offset sequence, adding complexity to the encryption. Achieve diverse encryption results through different displacement step combinations. The ciphertext contains offset sequence codes, ensuring that the decryption process is straightforward and accurate. This encryption method is suitable for scenarios that require enhanced security while maintaining the ease of implementation of Caesar Code.

Tips: This tool's dependency on JavaScript is not carried outConfusion, because it is used to open source to display code composition. Although it's enough to post on SNS or play a decryption game (when others don't know about this site) lol. If you want to actually use simple text encryption, pleaseRegenerate the offset sequenceWithDisplacement step table, and utilize the tool for JavaScript codeConfusion。
