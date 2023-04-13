class Solution {
    public boolean isValid(String s) {
        Stack<Character> stack = new Stack<Character>();

        switch (s.charAt(0)) {
            case ')':
            case ']':
            case '}':
                return false;
        }

        for (int i = 0; i < s.length(); i++) {
            switch (s.charAt(i)) {
                case '(':
                    stack.push('(');
                    break;
                case '[':
                    stack.push('[');
                    break;
                case '{':
                    stack.push('{');
                    break;
                case ')':
                    if (stack.empty() && i == s.length() - 1 || !stack.empty() && stack.pop() != '(')
                        return false;
                    break;
                case ']':
                    if (stack.empty() && i == s.length() - 1 || !stack.empty() && stack.pop() != '[')
                        return false;
                    break;
                case '}':
                    if (stack.empty() && i == s.length() - 1 || !stack.empty() && stack.pop() != '{')
                        return false;
                    break;
            }

        }
        if (!stack.empty())
            return false;
        return true;
    }
            
}
